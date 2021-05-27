# GomaNX v12.0.2-2 por Goma

## Compatibilidade: firmware 12.0.2 ou inferior 

Obrigado por utilizar o GomaNX! 

Meu objetivo com este pacote é simplificar a vida de quem está começando a hackear seu Nintendo Switch ou quem simplesmente quer atualizar seu desbloqueio de forma prática.

Se você estiver começando a hackear seu Switch, recomendo a leitura desse guia mais detalhado que escrevi: <http://guide.gomanx.me/>

Tentarei, de acordo com minhas possibilidades, disponibilizar novas versões deste pacote sempre que houverem lançamentos relevantes na cena de hacking do Switch.
O pacote é 100% gratuito e a versão mais recente dele sempre estará disponível em http://gomanx.me/

Para utilizar este pacote, basta copiar todo o conteúdo da pasta indicada para a raíz do seu cartão SD e injetar a payload do Hekate inclusa pelo seu injetor de preferência (TegraRcmGUI, Rekado, dongle etc.).
Visando simplificar, incluí no pacote também a última versão do TegraRcmGUI Portable com o Hekate já configurado como payload favorita.
O TegraRcmGUI às vezes não funciona em alguns computadores, então incluo também a versão instalável.

A fim de evitar conflitos, evite misturar esse pacote com outras CFWs no cartão SD. 
Idealmente, mantenha apenas seus arquivos importantes (pasta Nintendo, licença do SX OS, EmuNANDs, prodinfo etc.) e apague o todo resto antes de instalar pela primeira vez.
Se estiver atualizando seu pacote, a menos que especificado no changelog da versão, você pode apenas substituir os arquivos do pacote novo pelos antigos do SD.

É EXTREMAMENTE RECOMENDADO que seu cartão esteja formatado em FAT32, a fim de evitar corrupções de arquivos - ainda mais se você for utilizar EmuNAND.
Para formatá-lo em FAT32, use o software GUIformat incluso no pacote. Selecione seu cartão SD e Allocation Unit Size de 32768.
Certifique-se de fechar quaisquer janelas do Windows Explorer que estiverem abertas, ou o GUIformat retornará erro. Se ainda assim tiver erros, tente reiniciar o Windows Explorer pelo Task Manager (CTRL + ALT + DEL) ou reiniciar o PC.

O pacote vai configurado para bootar o menu do Hekate com sua interface gráfica Nyx.
Por essa interface, você pode realizar backup da sua NAND ou restaurar um backup, criar ou configurar sua(s) EmuNAND(s) (EmuMMC), habilitar AutoRCM, entre outras coisas úteis.
Para iniciar uma CFW no Hekate, navegue até Launch e escolha sua CFW de preferência. É possível também bootar o console na firmware oficial.

O AtmosphereCOTE JÁ VEM CONFIGURADO PARA OCULTAR A SUA PRODINFO AUTOMATICAMENTE. O USO DO INCOGNITO NÃO SE FAZ MAIS NECESSÁRIO.

## Conteúdo

Segue uma lista do que o pacote inclui, com os links para baixar tudo direto das respectivas fontes.

1. BOOTLOADER

    - [Hekate 5.5.6 + Nyx 1.0.3](https://github.com/CTCaer/hekate/releases)

    &nbsp;
2. CFW

    - [Atmosphere](https://github.com/Atmosphere-NX/Atmosphere/releases)

    &nbsp;
3. HOMEBREWS

    - [Homebrew App Store](https://www.switchbru.com/appstore/)
    - [Checkpoint](https://github.com/FlagBrew/Checkpoint/releases)
    - [EdiZon](https://github.com/WerWolv/EdiZon/releases)
    - [Lockpick_RCM](https://github.com/shchmue/Lockpick_RCM/releases)
    - [Homebrew Menu](https://github.com/switchbrew/nx-hbmenu/releases) 
    - [AIO-switch-updater](https://github.com/HamletDuFromage/AIO-switch-updater)

    - [Tinfoil](https://tinfoil.io/Download#download)
        - locations.conf
            - [Party Shop](https://partyshop.xyz); 
            - [Turtle Shop](https://tiny.cc/turtleshop e https://titz.ga/);
            - [UnderPrivlidged Shop UPStash](http://rebrand.ly/UPStash)
            - [UnderPrivlidged Shop UnderBack](http://rebrand.ly/UnderBack)
            - [Pengu's Shop](http://pengu.ga/)
            - [Stealth Shop](http://stealthshop.ga)
            - [Quota Shop](http://quotashop.ml)
            - [ReDUMP Shop](https://redump.ga/)

    - ~~[GomaNX Toolbox](https://github.com/AtlasNX/Kosmos/releases) (Fork do Kosmos Toolbox)~~
    - ~~[ldnmitm_config](https://github.com/spacemeowx2/ldn_mitm/releases)~~
    - ~~[Moonlight-NX](https://github.com/rock88/moonlight-nx/releases)~~
    - ~~[NX-Activity-Log](https://github.com/tallbl0nde/NX-Activity-Log)~~
    - ~~[NXThemesInstaller](https://github.com/exelix11/SwitchThemeInjector/releases)~~
    - ~~[nxmtp](https://github.com/liuervehc/nxmtp/releases)~~
    - ~~[NX-Shell](https://github.com/joel16/NX-Shell/releases)~~
    - ~~[Reset Parental Controls](https://github.com/ITotalJustice/Reset-Parental-Controls-NX/releases)~~

    &nbsp;  
4. Modulos de sistema Tesla Atmosphere (podem ser habilitados ou desabilitados pelo homebrew GomaNX Toolbox):~~

    - [Tesla](https://github.com/WerWolv/Tesla-Menu/releases)
    - [nx-ovlloader](https://github.com/WerWolv/nx-ovlloader/releases)
    - [ovlSysmodules](https://github.com/WerWolv/ovl-sysmodules/releases)
    - [Mission Control](https://github.com/ndeadly/MissionControl/releases)
    - [Emuiibo](https://github.com/XorTroll/emuiibo/releases)
    - [sys-ftpd-light](https://github.com/cathery/sys-ftpd-light/releases)
    - [sys-clk](https://github.com/retronx-team/sys-clk/releases)
    - [sys-clk-Overlay](https://github.com/Sun-Research-University/sys-clk-Overlay/releases)

    - ~~[ldn_mitm](https://github.com/spacemeowx2/ldn_mitm/releases)~~
    - ~~[sys-con](https://github.com/cathery/sys-con/releases)~~
    - ~~[sys-screenuploader](https://github.com/bakatrouble/sys-screenuploader/releases)~~
    - ~~[SysDVR](https://github.com/exelix11/SysDVR/releases)~~
    - ~~[Sys-Botbase](https://github.com/olliz0r/sys-botbase/releases)~~
    - ~~[nx-btred](https://github.com/plutooo/nx-btred/releases/)~~
    - ~~[Status Monitor Overlay](https://github.com/masagrator/Status-Monitor-Overlay/releases)~~
    - ~~[SaltyNX](https://github.com/masagrator/SaltyNX/releases)~~
    - ~~[ReverseNX-RT](https://github.com/masagrator/ReverseNX-RT/releases)~~
    - ~~[sys-tune](https://github.com/HookedBehemoth/sys-tune/releases)~~

    &nbsp;
5. Software para uso no PC

    - [TegraRcmGUI](https://github.com/eliboa/TegraRcmGUI/releases)
    - [GUIformat](http://www.ridgecrop.demon.co.uk/index.htm?guiformat.htm)
    - [Nut](https://github.com/blawar/nut/releases)
    - [Emutool](https://github.com/XorTroll/emuiibo/releases)
    - [Switch Theme Injector](https://github.com/exelix11/SwitchThemeInjector/releases)
    - [NRO2NSP + keys](https://github.com/Root-MtX/Nro2Nsp/releases)
    - [4NXCI + keys](https://github.com/The-4n/4NXCI/releases)
    - [NxNandManager](https://github.com/eliboa/NxNandManager/releases)
    - [PKHeX + Plugins](https://github.com/architdate/PKHeX-Plugins/releases/)
