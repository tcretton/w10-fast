# Scripts e dicas para Windows fast & secure - [**Baboo**](baboo.com.br)

[Artigo completo](https://www.baboo.com.br/windows-10/conteudo-essencial-windows/script-que-substitui-o-ccleaner/)

Scripts e dicas para manter o Windows, rápido e seguro. Compiladas do curso Windows rápido e seguro "Baboo"

- Script para apagar arquivos temporários
  Script substitui o CCleaner, não apaga cookies, nem histórico e senhas, deve ser executado via Prompt de Comando (Admin).
  Também pode ser executado via Agendador de Tarefas, funciona por usuário, ele não apaga os arquivos temporários de outros usuários, o ideal é rodar a cada 15 dias.
  Se você quiser executar o script e logo em seguida desligar automaticamente o computador, antes do final do script adicione a linha: `shutdown /t 30 /s`

# Passo a passo para Windows Rápido e Seguro

## 1 - Analise & Repair - HD & SSD

Western Digital Data LifeGuard
Western Digital Dashboard
Chkdsk
CHKDSK /R <Enter>
SFC Online
SFC /Scannow <Enter>
SFC Off-line Configurações > Atualização e Segurança > Recuperação > Reiniciar Agora… Solução de Problemas > Opções Avançadas > Prompt de Comando… Informe Login e Senha:
BCDEDIT
sfc /scannow /offbootdir=C:\ /offwindir=C:\windows <Enter>
Dism
DISM /Online /Cleanup-image /Restorehealth <Enter>

## 2 - Clean & Remove - Bloatware, Adware, Malware

Limpeza de Disco
script-clean
Adwcleaner
Desinstalar programas desnecessários
Verificação Tripla de Malware On Line TrendMicro Housecall - HouseCall KVRT Kapersky - KVRT ESET Online Scanner - ESET Scanner
Instalar Antivirus Panda free ou Kapersky
Bloquear Propaganda & URL Ublock Origin / Ublock Extra / Traffic Light Bit Defender / Kapersky Protection - link / Windows Defender Browser Protection / MalwareBytes Browser Guard MalwareBytes
Desfragmentar Defragler
Script para apagar arquivos temporários - “Baboo”
Fonte: Artigo Baboo.com.br

Script substitui o CCleaner, não apaga cookies, histórico e senhas, deve ser executado como Admin. Pode ser executado via Agendador de Tarefas, funciona por usuário, é ideal rodar a cada 15 dias. Se quiser executar o script e logo em seguida desligar automaticamente, antes do final do script adicione a linha: shutdown /t 30 /s

## 3 - Bloquear sites de download

Edite o arquivo hosts que esta na pasta C:\Windows\System32\drivers\etc

#IPv4

127.0.0.1 www.baixaki.com.br

127.0.0.1 baixaki.com.br

127.0.0.1 superdownloads.com.br

127.0.0.1 www.superdownloads.com.br

127.0.0.1 superd.com.br

127.0.0.1 www.superd.com.br

127.0.0.1 ultradownloads.com.br

127.0.0.1 www.ultradownloads.com.br

127.0.0.1 download.com

127.0.0.1 www.download.com

127.0.0.1 softpedia.com

127.0.0.1 www.softpedia.com

127.0.0.1 softonic.com

127.0.0.1 www.softonic.com

# IPv6

fe80::1%lo0 www.baixaki.com.br

fe80::1%lo0 baixaki.com.br

fe80::1%lo0 superdownloads.com.br

fe80::1%lo0 www.superdownloads.com.br

fe80::1%lo0 superd.com.br

fe80::1%lo0 www.superd.com.br

fe80::1%lo0 ultradownloads.com.br

fe80::1%lo0 www.ultradownloads.com.br

fe80::1%lo0 download.com

fe80::1%lo0 www.download.com

fe80::1%lo0 softpedia.com

fe80::1%lo0 www.softpedia.com

fe80::1%lo0 softonic.com

fe80::1%lo0 www.softonic.com
