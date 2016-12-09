# Wipe drive clean:
> cryptsetup open --type plain /dev/sdXY container --key-file /dev/random
> fdisk -l
> dd if=/dev/zero of=/dev/mapper/container status=progress
> cryptsetup close container

# Make partitions
> fdisk /dev/sdb
use GPT partition table
mark /boot as bootable

# Prepare and mount crypted partition
> cryptsetup -y -v luksFormat /dev/sdaX
> cryptsetup open /dev/sdaX cryptroot
> mkfs -t ext4 /dev/mapper/cryptroot
> mount -t ext4 /dev/mapper/cryptroot /mnt

# Check it
> umount /mnt
> cryptsetup close cryptroot
> cryptsetup open /dev/sdaX cryptroot
> mount -t ext4 /dev/mapper/cryptroot /mnt

# Install
> pacstrap /mnt base vim tmux wireless_tools iw wpa_supplicant dialog base-devel
> genfstab -U /mnt >> /mnt/etc/fstab
> arch-chroot /mnt

# Configure
> ln -s /usr/share/zoneinfo/Europe/Budapest /etc/localtime
> hwclock --systohc
> vim /etc/locale.gen
> locale-gen

> vim /etc/hostname
> vim /etc/hosts

> vim /etc/mkinitcpio.conf
-- put encrypt hook after udev before filesystems
> mkinitcpio -p linux

> passwd

# Config bootloader
> pacman -S intel-ucode grub
> blkid (read UUID)
> vim /etc/default/grub
GRUB_CMDLINE_LINUX="cryptdevice=UUID=<device-UUID>:cryptroot root=/dev/mapper/cryptroot"
> grub-install --target=i386-pc /dev/sdx
> grub-mkconfig -o /boot/grub/grub.cfg
