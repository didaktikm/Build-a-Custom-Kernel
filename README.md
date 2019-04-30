# Задача №1 Сборка собственного ядра для CenOS 7

## 1. Информачия о системе.

```
   sudo -i
   cat /etc/*rel*
   uname -r
```   

## 2. Подготовка системы. Установка необходимых пакетов для компиляции ядра.

### Загружаем необходимые пакеты.
```
   yum groupinstall "Development Tools"
   yum install ncurses-devel
   yum install hmaccalc zlib-devel binutils-devel elfutils-libelf-devel
```
### Переходим в директорию для сборки и загружаем исходники ядра.
```
   cd /usr/src/kernels
```   
Переходим на [www.kernel.org](https://www.kernel.org) нажимаем правой клавишей на *Latest Stable Kernel* и копируем адрес ссылки

![alt-текст](https://www.kernel.org/theme/images/icons/downloadarrow_small.png "Latest Stable Kernel")
