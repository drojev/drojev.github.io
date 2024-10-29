---
title: Iniciando un laboratorio de Ethical Hacking
layout: post
published: true
tags: [ciberseguridad, vbox, tutorial]
date: 2024-10-29 01:38:00 -0000
---

# Topología e instalación del laboratorio de trabajo - Ethical Hacking

## Introducción

En este tutorial, aprenderás a crear un laboratorio de ethical hacking utilizando VirtualBox. Este entorno te permitirá practicar habilidades de ciberseguridad de manera segura.

## Topología del Laboratorio

Nuestro entorno de trabajo contará con un atacante, víctima y una maquina metasploitable. Todas las maquinas que intervengan en nuestra topología serán elementos virtualizados en VMware o Virtualbox.

![Descripción de la imagen]({{ site.baseurl }}/assets/images/laboratorio/topologia.png)


## Instalación y comunicación entre maquinas virtuales
Para la implementación de los maquinas virtualizadas instalaremos Virtualbox.

Desde aquí puede instalar [Virtualbox v6.1.26](https://download.virtualbox.org/virtualbox/6.1.26/VirtualBox-6.1.26-145957-Win.exe) desde la página oficial del software.

### Paso 1: Instalar Virtualbox

Una vez que haya descargado Virtualbox procederemos a instalarlo.

*Nota: si es la primera vez que emplea maquinas virtuales, debe habilitar la funcionalidad de virtualización a través de la BIOS/UEFI  de su ordenador.*


<div style="text-align: center;">
    <img src="{{ site.baseurl }}/assets/images/laboratorio/vbox.png" alt="Descripción de la imagen" />
</div>


### Paso 2: Instalación de Kali Linux en Virtualbox

- Descargamos [Kali Linux v2022.2](https://kali.download/virtual-images/kali-2022.2/kali-linux-2022.2-virtualbox-amd64.ova) desde la página oficial.

- Importamos el archivo *.ova* en Virtualbox y procederemos con la instalación de Kali Linux con las configuraciones predeterminadas.

  *username: kali, password: kali*


 | ![Descripción de la imagen]({{ site.baseurl }}/assets/images/laboratorio/topologia.png) | ![Descripción de la imagen]({{ site.baseurl }}/assets/images/laboratorio/topologia.png) |

### Paso 3: Instalación de la maquina metasploitable

- Procedemos con la descarga de [Metasploitable2](https://sourceforge.net/projects/metasploitable/files/latest/download) y su instalación en Virtualbox.

- Una vez que importamos el disco procedemos a iniciar la virtualización.

### Paso 4: Instalación de Windows 7 en Virtualbox

- Procedemos con la descarga de la extensión *.iso* de [Windows 7](https://getintopc.com/softwares/operating-systems/windows-7-ultimate-download-iso-32-bit-64-bit-official-free-1585306/) y su instalación.

- Luego de crear la maquina virtualizada procederemos a iniciar windows. 

### Paso 5: Prueba de comunicación entre maquinas virtualizadas

- Realizar pruebas de ICMP entre las maquinas virtualizadas.

  *Realizar la configuración de red en Virtualbox en modo "bridge"*

