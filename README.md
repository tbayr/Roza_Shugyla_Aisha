# Roza_Shugyla_Aisha
final_commands
Task1:
sudo su
useradd student
passwd student
login student 
whoami
logout
exit

Task2:
ping 142.250.180.110
proxychains curl https://moodle.astanait.edu.kz/ -v
ping youtube.com
ifconfig 

Task3:
apt-get install build-essential linux-headers-$(uname -r)
nano final.c
MODULE_LICENCE("GPL");
MODULE_AUTHOR("ROZA");
MODULE_DESCRIPTION("KERNEL MODULE");
MODULE_VERSION("0.1");
static int __init hello_init(void) {
      printk(KERNEL_INFO "Loading HEllo Module... \n");
      printk(KERNEL_INFO "Hello World\n");
      return 0;
} 
static void __exit hello_exit(void) {
      printk(KERNEL_INFO "Goodbye World\n");
}
module_init(hello_init);
module_exit(hello_exit);

ls
cat Makefile
make -C /lib/modules/$(shell uname -r)/build M=$(pwd) modules
ls
sudo insmod my_module.ko
lsmod | grep my_module

