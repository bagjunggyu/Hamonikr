# Hamonikr
하모니카를 만들 때 사용했던 설정을 정리해둔 페이지입니다.

Linux Mint Mate 꾸미기

* plank theme - pantheon

* plank 에 둘 런처들 (왼쪽 부터 오른쪽 순으로)
파이어 폭스, thunderbird, 파일 브라우저, 터미널, pluma, 마테 이미지 뷰어, 클레멘타인, smplayer, 계산기, slingscold, synapse, 제어 센터

* 패널 투명도 수정 - 완전 투명하게

* Covergloobus 위치 : 가운데, 오른쪽 끝 부분 , tilda 를 열면 화면 오른쪽 끝부분에서 tilda 두께의 중앙에 위치하면 됨 


* 테마 설정
컨트롤 - VoyagerX-1 : 추가되는 테마
창 가장자리 - Paper : 추가되는 테마
아이콘 - Awoken
포인터 - oxy-white : 추가되는 포인터 테마
글꼴 크기 : 10

Voyager X 테마
https://dl.dropboxusercontent.com/    u/54450962/voyagerx-themes.tar.gz

* Tilda 설정
크기 : 가로 - 100%, 세로 - 33% 
위치 : 좌,우 모두 중앙
투명도 :  33%

* 터미널 프로파일 설정 테마 바뀜
색 - 시스템 테마 색 사용
배경 - 없음

* 제거 할 프로그램 - gThumb 
gthumb를 대신할 만한 프로그램은 Shotwell 입니다.
apt install shotwell

xcompmgr을 대신해서 컴포지팅 사용
제어판 - 개인 - 데스크톱 설정 - 창의 성능에서 '컴포지팅 사용'을 하면 그 효과를 보이며,
제어판- 개인 - 창 - 위치 의 창 맞추기에서 '가장자리 별로 바둑판 배치 활성화를 하면 
마테에서 부족했던 윈도우 액션이 가능해 집니다.


* 배경화면 추가 - Francisco 의 사진중에서 2개 추가 
(Xubuntu 14.04에 쓰이는 사진중에 하나를 제공한 사람)

* 시작 메뉴 즐겨 찾기에 등록될 9개 런처
(왼쪽 위부터 오른쪽 아래줄 순으로)
Gparted, Bleachbit, 시동 디스크 생성기
타임 시프트, 부트 리페어, Grub-Customizer
Transmission, 스크린샷, Kazam

* 추가되는 프로그램들
오래된 캐시 정리 도구 Bleachit)
apt install bleachbit

Grub 정리 도구 Grub-Customizer)
sudo add-apt-repository ppa:danielrichter2007/grub-customizer -y;apt update;apt install grub-customizer -y

빠른 검색 도구 Synapse)
참고 : http://bagjunggyu.blogspot.kr/2015/03/synapse.html
sudo apt-add-repository ppa:synapse-core/ppa -y;sudo apt update;sudo apt install synapse -y

전체 어플 빠르게 보는 도구 Slingscold)
http://blog.daum.net/bagjunggyu/183
sudo add-apt-repository ppa:noobslab/apps -y;apt update;apt install slingscold-launcher -y

iPad 충전)
sudo apt-add-repository ppa:heathbar/ipad-charge -y;sudo apt-get update;sudo apt-get install libusb-1.0-0 ipad-charge -y

touchpad-indicator)
sudo apt-add-repository ppa:atareao/atareao -y;sudo apt-get update;sudo apt-get install touchpad-indicator -y

* 단축키 설정 변화
추가되는 단축키 지정 어플)
윈도우의 긴급 태스크 종료 Ctrl + Alt + Delete 와 같은 기능
프로그램 이름 : mate-system-monitor
단축키 : Super + Alt + Delete

시작 메뉴 단축키 바뀜 ( Mint 13 시절의 단축키)
Ctrl_L + Super

synapse 단축키)
Super + Space

Slingscold 단축키)
Ctrl + Space

Super + 숫자 : 메뉴의 단축키를 Ctrl_L + Super 로 해서 Super 키가 자유로워짐
Super + 1 = 웹브라우저 - 기본 지정키 변경
Super + 2 = 파일 브라우저 - 기본 지정 키 변경
Super + 3 = 음악 플레이어 - 기본 지정 키 변경
Super + 4 = SMplayer - 별도 추가 지정

* 커서 아이콘 추가
https://drive.google.com/file/d/0Bxy-IhcjQjbDX21YSDVRNVBEU0U/view?usp=sharing
cursor-icons 안의 여러 커서 아이콘 폴더들
/usr/share/icons

* 시작 메뉴 아이콘 바꿈 
시작 메뉴에 쓰일 만한 3개의 아이콘들 

https://drive.google.com/file/d/0Bxy-IhcjQjbDV0ZsNVpKd0NqaVk/view?usp=sharing

/uar/share/icons/menu-sky.png

또는 바탕 화면 보기를 아이콘 대신 쓰며 맨 왼쪽에 둠

paper theme)
sudo add-apt-repository ppa:snwh/pulp -y;sudo apt-get update;sudo apt-get install paper-gtk-theme -y

* aliases
alias 설치='sudo apt-get install -y'
alias 모두설치='sudo dpkg -i *.deb'
alias 제거='sudo apt-get remove -y'
alias 자동제거='sudo apt-get autoremove --purge -y'
alias 다시='sudo reboot'
alias 끔='sudo shutdown -hP'
alias 업뎃=’sudo apt-get update’
alias 업그리='sudo apt-get update;sudo apt-get dist-upgrade -y'
alias 업글='sudo apt-get update;sudo apt-get upgrade -y'
alias 닫기='exit'
alias 정리='clear'
alias 캐시정리='sudo apt-get autoclean'
alias 보기='ls'
alias 복사='cp'
alias 이사='mv'
alias 이동='cd'
alias 이름='mv'
alias 수지='sudo pluma'
alias 찾기='sudo apt-cache search'
alias 추가='sudo apt-add-repository -y'
alias pl='pluma'
alias deb=’sudo dpkg -i’
alias add='sudo apt-add-repository -y'
alias reboot='sudo reboot'
alias install='sudo apt-get install -y'
alias remove='sudo apt-get remove -y'
alias update='sudo apt-get update -y'
alias upgrade='sudo apt-get upgrade -y'
alias dist-upgrade='sudo apt-get update;sudo apt-get dist-upgrade -y'
alias search='sudo apt-cache search'
alias autoremove='sudo apt-get autoremove --purge -y'
alias autoclean='sudo apt-get autoclean -y'
alias 크롬설치=’sudo apt-get install google-chrome-stable -y’
alias 크롬제거=’sudo apt-get remove google-chrome-stable -y’
alias Rma=’sudo shutdown -hP’
alias ektl=’sudo reboot’

* 영어로 설치한 OS 한글로 바꾸기
http://bagjunggyu.blogspot.kr/2015/03/os.html
내용중에 한국 설정 패키지들을 확인해주세요

* 멋진 디지털 그림 도구 크리타(Ktria) alias에 반영
http://bagjunggyu.blogspot.kr/2015/03/krita.html
alias 크리타설치='sudo apt-get install krita kritasketch kdelibs-bin kde-style-oxygen -y'

* compiz 설정하기 
http://bagjunggyu.blogspot.kr/2015/04/linux-mint-17-mate-compiz.html


* swappiness 조절
sudo pluma /etc/sysctl.conf

열린 문서의 맨 아래에 아래 문장들을 추가 & 저장 하시고 재부팅 하면 됩니다.

# Decrease swap usage to a reasonable level
vm.swappiness=10
# Improve cache management
vm.vfs_cache_pressure=50

* ppa들입니다.

제어판 - 소프트웨어소스 에서 해당 항목에 추가 하시며 됩니다.

<추가 저장소>
구글 크롬 브라우저
deb http://dl.google.com/linux/chrome/deb/ stable main

AwOken 아이콘 테마)
deb http://ppa.launchpad.net/alecive/antigone/ubuntu trusty main
터치패드 사용 설정 도구 Touchpad-Indicator)
deb http://ppa.launchpad.net/atareao/atareao/ubuntu trusty main

Grub-Customizer)
deb http://ppa.launchpad.net/danielrichter2007/grub-customizer/ubuntu trusty main

미디어 플레이어 Bomi)
deb http://ppa.launchpad.net/darklin20/bomi/ubuntu trusty main

iPad 충전기)
deb http://ppa.launchpad.net/heathbar/ipad-charge/ubuntu trusty main

음악 플레이어 Clementine)
deb http://ppa.launchpad.net/me-davidsansome/clementine/ubuntu trusty main

Emerald Compiz 창 꾸미기 테마 와 도구)
deb http://ppa.launchpad.net/nilarimogard/webupd8/ubuntu trusty main

Slingcold (슬링샷) 전체 프로그램 접근 도구 - 패널 버전입니다)
deb http://ppa.launchpad.net/noobslab/apps/ubuntu trusty main

Numix 테마 와 아이콘)
deb http://ppa.launchpad.net/numix/ppa/ubuntu trusty main

Plank 런처 도크)
deb http://ppa.launchpad.net/ricotz/docky/ubuntu trusty main

미디어 플레이어 SMplayer) 
deb http://ppa.launchpad.net/rvm/smplayer/ubuntu trusty main

Paper 테마)
deb http://ppa.launchpad.net/snwh/pulp/ubuntu trusty main

빠른 검색 도구 Synapse)
deb http://ppa.launchpad.net/synapse-core/ppa/ubuntu trusty main

시스템 백업 및 복원 도구 Timeshift)
deb http://ppa.launchpad.net/teejee2008/ppa/ubuntu trusty main

부팅 복구 도구 Boot-repair)
deb http://ppa.launchpad.net/yannubuntu/boot-repair/ubuntu trusty main

디지털 페인팅 도구 Krita)
deb http://ppa.launchpad.net/kubuntu-ppa/backports/ubuntu trusty main

<개별 저장소 PPA> 
또는 터미널에서 sudo apt-add-repository 명령어를 이용하시려는 분들은
이렇게 이용하시면 됩니다.
위의 주소들에서 launchpad.net 다음의 슬래쉬(/) 부터는 이렇습니다.
/런치패드-사용자-아이디/프로젝트-이름/우분투 코드-네임 트리

이것을 이렇게 이용하시면 됩니다.
ppa:런치패드-사용자-아이디/프로젝트-이름 입니다.

개별 저장소에는 이렇게 ppa:noobslab/apps 
터미널에서는 이렇게 sudo apt-add-repository ppa:noobslab/apps
적용하시면 됩니다.

제거하는 --remove 옵션이 이젠 없네요....이전에는 되더니 안되더군요
하모니카에는 ppa 추가를 add 라고 줄여서 alias 로 지정해주었습니다.

sudo apt-add-repository ppa:alecive/antigone -y;sudo apt-add-repository ppa:atareao/atareao -y;sudo apt-add-repository ppa:caffeine-developers/ppa -y;sudo apt-add-repository ppa:danielrichter2007/grub-customizer -y;sudo apt-add-repository ppa:darklin20/bomi -y;sudo apt-add-repository ppa:heathbar/ipad-charge -y;sudo apt-add-repository ppa:me-davidsansome/clementine -y;sudo add-apt-repository ppa:nilarimogard/webupd8 -y;sudo apt-add-repository ppa:noobslab/apps -y;

sudo apt-add-repository ppa:numix/ppa -y;sudo apt-add-repository ppa:ricotz/docky -y;sudo apt-add-repository ppa:snwh/pulp -y;sudo apt-add-repository ppa:synapse-core/ppa -y;sudo apt-add-repository ppa:teejee2008/ppa -y;sudo apt-add-repository ppa:yannubuntu/boot-repair -y;sudo add-apt-repository ppa:kubuntu-ppa/backports -y;sudo add-apt-repository ppa:linrunner/tlp -y;sudo add-apt-repository ppa:team-xbmc/ppa -y;

sudo apt update;sudo apt install touchpad-indicator grub-customizer bomi libusb-1.0-0 ipad-charge clementine emerald slingscold numix-icon-theme-circle numix-gtk-theme plank smplayer paper-gtk-theme synapse timeshift boot-repair bleachbit kazam usb-creator-gtk tlp tlp-rdw shotwell fonts-noto-cjk gparted smplayer smplayer-themes smplayer-translations smtube kodi grub-customizer moc tilda -y

slingscold 와 synapse boot-repair timeshift bleachbit의 사용법은 이 글들을 참고해보세요

http://bagjunggyu.blogspot.kr/2015/03/slingscold.html
http://bagjunggyu.blogspot.kr/2015/03/synapse.html
http://bagjunggyu.blogspot.kr/2012/09/grub_29.html
http://bagjunggyu.blogspot.kr/2013/11/timeshift.html
http://bagjunggyu.blogspot.kr/2013/09/mintlunaubuntu-ubuntu.html

멋진 배경화면

Francisco Villarroel
http://bokehlicia.deviantart.com/

Flare Desktop Wallpaper
http://mariesturges.deviantart.com/art/Flare-for-Desktop-191407517

Rain Wallpaper
http://zomx.deviantart.com/art/Rain-Wallpaper-296661569

Rainbow Clouds Wallpaper
http://martz90.deviantart.com/art/Rainbow-Clouds-Wallpaper-299977599

<동영상>
https://youtu.be/Xc-mUluyEY8

썬더버드 부가기능 lightning(일정표 기능) 추가


