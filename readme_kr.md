﻿-----------------------1.0.0-----------------------

이 프로그램은 윈도우-우분투간의 부팅전환을 편리하게 만들기위해 제작되었습니다.
우분투 데스크톱, 윈도우즈 운영체제에서 구동이 가능하며 추가적인 설정이 필요합니다.


1. 우분투 설정

1-1. 받은 UBuntu 폴더를 원하는 경로로 저장합니다.

1-2. Windowsboot.desktop 파일을 데스크탑경로로 옮깁니다.

1-3. windowsboot.sh 의 내용중 "input your root password" 부분에 로컬컴퓨터의 root 비밀번호를 입력후 저장합니다.

1-4. grub.cfg파일을 삭제후,  로컬컴퓨터의 /boot/grub/grub.cfg 파일을 복사해옵니다.

1-5. grub.cfg의 내용중 set default="0" 을 본인 컴퓨터에 맞게 숫자를 변경해줍니다.

1-6. Windowsboot.desktop 파일의 Exec 부분을 본인 컴퓨터의 sh 파일경로로 설정해줍니다.

1-7. shell을 실행후, 'chmod +x windowsboot.sh' 명령어를 입력하여 실행권한을 줍니다.

-----------------------1.0.1-----------------------

2. 윈도우 설정

1-1. 받은 Windows 폴더를 원하는 경로로 저장합니다.

1-2. 그리고 http://ext2-volume-manager.en.lo4d.com/ 이 경로로 들어가서 프로그램을 받아서 ext3(우분투)볼륨을 마운트 시킵니다.

# windows 에서는 fat32,ntfs 외의 파일시스템을 읽지못해서 이 프로그램을 사용합니다.

1-3. 마운트시킨 볼륨에있는 /boot/grub/grub.cfg 파일을 복사해옵니다.

1-4. ubuntuboot.bat 의 내용중 "input your mount volumn /boot/grub/grub.cfg path" 부분에 마운트시킨 볼륨에있는 grub.cfg 경로를 입력합니다.

1-5. 그후 사용하기 편리하게 바탕화면에 바로가기를 만들어줍니다.

※제한사항
우분투와 윈도우를 멀티부트할경우 grub 부팅이 되어야 사용이 가능합니다.
윈도우에서는 ext2 volumn manger를 사용하여야, 프로그램 구동이 가능합니다.

