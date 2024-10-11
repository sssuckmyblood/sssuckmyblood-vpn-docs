**Шаг 1:** Получить профиль для подключения к серверу

<details>
  <summary>Установка NekoRay на ПК</summary>

  ## Установка программы и подключение к серверу
  - Скачать программу с оффициального репозитория https://github.com/MatsuriDayo/nekoray/releases/download/3.26/nekoray-3.26-2023-12-09-windows64.zip
  - Распаковать загруженный .zip файл в удобное место на вашем компьютере
  - Открыть распакованную папку и запустить файл nekoray.exe
  - Если при запуске выдает ошибку DLL скачать и установить vc_redist https://aka.ms/vs/17/release/vc_redist.x64.exe

  - После запуска nekoray.exe, скопировать профиль VLESS который я скинул, нажать Программа и добавить профиль из буфера обмена
   <p align="center">
  <img src="https://github.com/user-attachments/assets/2691ab29-dcf1-4ab3-9dd9-cb0a0b7c9b93" alt="Описание изображения" style="margin: 20px;"/>
 </p>
    
  - Далее правой кнопкой мыши по появившейся строке профиля и нажать Запустить, слева от строки профиля должна появиться галочка - профиль активен
   
    <p align="center">
    <img src="https://github.com/user-attachments/assets/16d032a5-9b0b-4248-8907-16f7ab350725" alt="Описание изображения" style="margin: 20px;"/>
    </p>

  - После этого выбрать режим TUN или режим системного прокси. Одно из двух, вместе они работать не будут. Сначала выбираем режим TUN, проверяем работает ли интернет и другие заблокированные сервисы. Если ничего не работает - пробуем режим системного прокси. Если и так ничего не работает - пишем мне.
   
    <p align="center">
    <img src="https://github.com/user-attachments/assets/717211b3-3ea6-445b-85a0-f3479894ed00" alt="Описание изображения" style="margin: 20px;"/>
    </p>
    
   ## Настройка маршрутизации

   - Сверху в программе нажимаем Настройки, выбираем строку Настройки маршрутов
     <p align="center">
     <img src="https://github.com/user-attachments/assets/2d630915-a0af-46a4-a13e-7241af2c6254" alt="Описание изображения" style="margin: 20px;"/>
     </p>
     
   - Далее следуем шагам на скрине. Outboud по-умолчанию должен быть bypass.
     
      <p align="center">
     <img src="https://github.com/user-attachments/assets/a352da1a-7cf6-46dc-b2f0-617fee74bbf1" alt="Описание изображения" style="margin: 20px;"/>
     </p>

   - В редакторе JSON слева удаляем весь текст и вставляем туда набор маршрутов (текст ниже)
       <p align="center">
       <img src="https://github.com/user-attachments/assets/9987ef4d-557f-4fb0-8628-564569023377" alt="Описание изображения" style="margin: 20px;"/>
      </p>
      <p align="center">
     <img src="https://github.com/user-attachments/assets/ca69450a-25b9-49cf-860c-26d05bd3da13" alt="Описание изображения" style="margin: 20px;"/>
      </p>
     
            {
                "rules": [
             {
                        "domain": [
                            "chatgpt.com",
                            "discord-attachments-uploads-prd.storage.googleapis.com",
                            "dis.gd",
                            "discord.co",
                            "discord.com",
                            "discord.design",
                            "discord.dev",
                            "discord.gg",
                            "discord.gift",
                            "discord.gifts",
                            "discord.media",
                            "discord.new",
                            "discord.store",
                            "discord.tools",
                            "discordapp.com",
                            "discordapp.net",
                            "discordmerch.com",
                            "discordpartygames.com",
                            "discord-activities.com",
                            "discordactivities.com",
                            "discordsays.com",
                            "discordstatus.com",
                            "latency.discord.media",
                            "youtube.com",
                            "googlevideo.com",
                            "ytimg.com",
                            "oaistatic.com",
                            "instagram.com",
                            "cdninstagram.com",
                            "facebook.com",
                            "fbcdn.net"
                        ],
                        "outboundTag": "proxy",
                        "type": "field"
                    },
                    {
                        "ip": [
                            "5.200.14.0/24",
                            "34.0.192.0/24",
                            "34.0.193.0/24",
                            "34.0.194.0/24",
                            "34.0.195.0/24",
                            "34.0.196.0/24",
                            "34.0.197.0/24",
                            "34.0.198.0/24",
                            "34.0.199.0/24",
                            "34.0.200.0/24",
                            "34.0.201.0/24",
                            "34.0.202.0/24",
                            "34.0.203.0/24",
                            "34.0.204.0/24",
                            "34.0.205.0/24",
                            "34.0.206.0/24",
                            "34.0.207.0/24",
                            "34.0.208.0/24",
                            "34.0.209.0/24",
                            "34.0.210.0/24",
                            "34.0.211.0/24",
                            "34.0.212.0/24",
                            "34.0.213.0/24",
                            "34.0.215.0/24",
                            "34.0.216.0/24",
                            "34.0.217.0/24",
                            "34.0.218.0/24",
                            "34.0.220.0/24",
                            "34.0.221.0/24",
                            "34.0.222.0/24",
                            "34.0.223.0/24",
                            "34.0.240.0/24",
                            "34.0.241.0/24",
                            "34.0.242.0/24",
                            "34.0.243.0/24",
                            "34.0.244.0/24",
                            "34.0.245.0/24",
                            "34.0.246.0/24",
                            "34.0.247.0/24",
                            "34.0.248.0/24",
                            "34.0.249.0/24",
                            "34.0.250.0/24",
                            "34.0.251.0/24",
                            "35.207.64.0/24",
                            "35.207.65.0/24",
                            "35.207.67.0/24",
                            "35.207.71.0/24",
                            "35.207.72.0/24",
                            "35.207.73.0/24",
                            "35.207.74.0/24",
                            "35.207.75.0/24",
                            "35.207.76.0/24",
                            "35.207.77.0/24",
                            "35.207.78.0/24",
                            "35.207.79.0/24",
                            "35.207.80.0/24",
                            "35.207.81.0/24",
                            "35.207.82.0/24",
                            "35.207.83.0/24",
                            "35.207.84.0/24",
                            "35.207.85.0/24",
                            "35.207.86.0/24",
                            "35.207.87.0/24",
                            "35.207.89.0/24",
                            "35.207.91.0/24",
                            "35.207.92.0/24",
                            "35.207.95.0/24",
                            "35.207.97.0/24",
                            "35.207.99.0/24",
                            "35.207.100.0/24",
                            "35.207.101.0/24",
                            "35.207.103.0/24",
                            "35.207.104.0/24",
                            "35.207.106.0/24",
                            "35.207.107.0/24",
                            "35.207.108.0/24",
                            "35.207.109.0/24",
                            "35.207.110.0/24",
                            "35.207.111.0/24",
                            "35.207.114.0/24",
                            "35.207.115.0/24",
                            "35.207.116.0/24",
                            "35.207.117.0/24",
                            "35.207.121.0/24",
                            "35.207.122.0/24",
                            "35.207.124.0/24",
                            "35.207.125.0/24",
                            "35.207.126.0/24",
                            "35.207.129.0/24",
                            "35.207.131.0/24",
                            "35.207.132.0/24",
                            "35.207.135.0/24",
                            "35.207.136.0/24",
                            "35.207.137.0/24",
                            "35.207.139.0/24",
                            "35.207.140.0/24",
                            "35.207.141.0/24",
                            "35.207.142.0/24",
                            "35.207.143.0/24",
                            "35.207.144.0/24",
                            "35.207.145.0/24",
                            "35.207.146.0/24",
                            "35.207.147.0/24",
                            "35.207.149.0/24",
                            "35.207.150.0/24",
                            "35.207.151.0/24",
                            "35.207.153.0/24",
                            "35.207.154.0/24",
                            "35.207.155.0/24",
                            "35.207.156.0/24",
                            "35.207.157.0/24",
                            "35.207.158.0/24",
                            "35.207.160.0/24",
                            "35.207.162.0/24",
                            "35.207.163.0/24",
                            "35.207.164.0/24",
                            "35.207.165.0/24",
                            "35.207.166.0/24",
                            "35.207.167.0/24",
                            "35.207.168.0/24",
                            "35.207.170.0/24",
                            "35.207.171.0/24",
                            "35.207.172.0/24",
                            "35.207.174.0/24",
                            "35.207.176.0/24",
                            "35.207.178.0/24",
                            "35.207.180.0/24",
                            "35.207.181.0/24",
                            "35.207.182.0/24",
                            "35.207.184.0/24",
                            "35.207.185.0/24",
                            "35.207.186.0/24",
                            "35.207.187.0/24",
                            "35.207.188.0/24",
                            "35.207.189.0/24",
                            "35.207.190.0/24",
                            "35.207.191.0/24",
                            "35.214.128.0/24",
                            "35.214.129.0/24",
                            "35.214.130.0/24",
                            "35.214.131.0/24",
                            "35.214.132.0/24",
                            "35.214.133.0/24",
                            "35.214.134.0/24",
                            "35.214.137.0/24",
                            "35.214.138.0/24",
                            "35.214.140.0/24",
                            "35.214.142.0/24",
                            "35.214.143.0/24",
                            "35.214.144.0/24",
                            "35.214.145.0/24",
                            "35.214.146.0/24",
                            "35.214.147.0/24",
                            "35.214.148.0/24",
                            "35.214.149.0/24",
                            "35.214.151.0/24",
                            "35.214.152.0/24",
                            "35.214.156.0/24",
                            "35.214.158.0/24",
                            "35.214.159.0/24",
                            "35.214.160.0/24",
                            "35.214.161.0/24",
                            "35.214.162.0/24",
                            "35.214.163.0/24",
                            "35.214.165.0/24",
                            "35.214.167.0/24",
                            "35.214.169.0/24",
                            "35.214.170.0/24",
                            "35.214.171.0/24",
                            "35.214.172.0/24",
                            "35.214.173.0/24",
                            "35.214.175.0/24",
                            "35.214.177.0/24",
                            "35.214.179.0/24",
                            "35.214.180.0/24",
                            "35.214.181.0/24",
                            "35.214.184.0/24",
                            "35.214.185.0/24",
                            "35.214.186.0/24",
                            "35.214.187.0/24",
                            "35.214.191.0/24",
                            "35.214.192.0/24",
                            "35.214.193.0/24",
                            "35.214.194.0/24",
                            "35.214.195.0/24",
                            "35.214.196.0/24",
                            "35.214.197.0/24",
                            "35.214.198.0/24",
                            "35.214.199.0/24",
                            "35.214.201.0/24",
                            "35.214.203.0/24",
                            "35.214.204.0/24",
                            "35.214.205.0/24",
                            "35.214.207.0/24",
                            "35.214.208.0/24",
                            "35.214.209.0/24",
                            "35.214.210.0/24",
                            "35.214.211.0/24",
                            "35.214.212.0/24",
                            "35.214.213.0/24",
                            "35.214.214.0/24",
                            "35.214.215.0/24",
                            "35.214.216.0/24",
                            "35.214.217.0/24",
                            "35.214.218.0/24",
                            "35.214.219.0/24",
                            "35.214.220.0/24",
                            "35.214.221.0/24",
                            "35.214.222.0/24",
                            "35.214.223.0/24",
                            "35.214.224.0/24",
                            "35.214.225.0/24",
                            "35.214.226.0/24",
                            "35.214.227.0/24",
                            "35.214.228.0/24",
                            "35.214.229.0/24",
                            "35.214.231.0/24",
                            "35.214.233.0/24",
                            "35.214.235.0/24",
                            "35.214.237.0/24",
                            "35.214.238.0/24",
                            "35.214.239.0/24",
                            "35.214.240.0/24",
                            "35.214.241.0/24",
                            "35.214.243.0/24",
                            "35.214.244.0/24",
                            "35.214.245.0/24",
                            "35.214.246.0/24",
                            "35.214.248.0/24",
                            "35.214.249.0/24",
                            "35.214.250.0/24",
                            "35.214.251.0/24",
                            "35.214.252.0/24",
                            "35.214.253.0/24",
                            "35.214.255.0/24",
                            "35.217.0.0/24",
                            "35.217.1.0/24",
                            "35.217.2.0/24",
                            "35.217.3.0/24",
                            "35.217.4.0/24",
                            "35.217.5.0/24",
                            "35.217.6.0/24",
                            "35.217.8.0/24",
                            "35.217.9.0/24",
                            "35.217.11.0/24",
                            "35.217.12.0/24",
                            "35.217.14.0/24",
                            "35.217.15.0/24",
                            "35.217.16.0/24",
                            "35.217.17.0/24",
                            "35.217.18.0/24",
                            "35.217.19.0/24",
                            "35.217.20.0/24",
                            "35.217.21.0/24",
                            "35.217.22.0/24",
                            "35.217.23.0/24",
                            "35.217.24.0/24",
                            "35.217.25.0/24",
                            "35.217.26.0/24",
                            "35.217.27.0/24",
                            "35.217.28.0/24",
                            "35.217.29.0/24",
                            "35.217.30.0/24",
                            "35.217.31.0/24",
                            "35.217.32.0/24",
                            "35.217.33.0/24",
                            "35.217.35.0/24",
                            "35.217.36.0/24",
                            "35.217.37.0/24",
                            "35.217.38.0/24",
                            "35.217.39.0/24",
                            "35.217.40.0/24",
                            "35.217.41.0/24",
                            "35.217.43.0/24",
                            "35.217.45.0/24",
                            "35.217.46.0/24",
                            "35.217.47.0/24",
                            "35.217.48.0/24",
                            "35.217.49.0/24",
                            "35.217.50.0/24",
                            "35.217.51.0/24",
                            "35.217.52.0/24",
                            "35.217.53.0/24",
                            "35.217.54.0/24",
                            "35.217.55.0/24",
                            "35.217.56.0/24",
                            "35.217.57.0/24",
                            "35.217.58.0/24",
                            "35.217.59.0/24",
                            "35.217.60.0/24",
                            "35.217.61.0/24",
                            "35.217.62.0/24",
                            "35.217.63.0/24",
                            "35.219.225.0/24",
                            "35.219.226.0/24",
                            "35.219.227.0/24",
                            "35.219.228.0/24",
                            "35.219.229.0/24",
                            "35.219.230.0/24",
                            "35.219.231.0/24",
                            "35.219.235.0/24",
                            "35.219.236.0/24",
                            "35.219.238.0/24",
                            "35.219.239.0/24",
                            "35.219.241.0/24",
                            "35.219.242.0/24",
                            "35.219.243.0/24",
                            "35.219.244.0/24",
                            "35.219.245.0/24",
                            "35.219.246.0/24",
                            "35.219.247.0/24",
                            "35.219.248.0/24",
                            "35.219.249.0/24",
                            "35.219.251.0/24",
                            "35.219.252.0/24",
                            "35.219.253.0/24",
                            "35.219.254.0/24",
                            "66.22.196.0/24",
                            "66.22.197.0/24",
                            "66.22.198.0/24",
                            "66.22.199.0/24",
                            "66.22.216.0/24",
                            "66.22.217.0/24",
                            "66.22.238.0/24",
                            "66.22.241.0/24",
                            "66.22.243.0/24",
                            "66.22.244.0/24"
                        ],
                        "network": [
                            "udp"
                        ],
                        "outboundTag": "proxy",
                        "type": "field"
                    },
                    {
                        "ip": [
                            "0.0.0.0/0",
                            "::/0"
                        ],
                        "outboundTag": "direct",
                        "type": "field"
                    }
                ]
            }
     
     - Если какие-то игры не работают с данным набором маршрутизации (у меня например Apex Legens не загружался), тогда меняем набор на следующий (порядок действий как в прошлом пункте, только копируем текст ниже)
       ```
           {
        "rules": [
            {
                "domain": [
                    "chatgpt.com",
                    "discord-attachments-uploads-prd.storage.googleapis.com",
                    "dis.gd",
                    "discord.co",
                    "discord.com",
                    "discord.design",
                    "discord.dev",
                    "discord.gg",
                    "discord.gift",
                    "discord.gifts",
                    "discord.media",
                    "discord.new",
                    "discord.store",
                    "discord.tools",
                    "discordapp.com",
                    "discordapp.net",
                    "discordmerch.com",
                    "discordpartygames.com",
                    "discord-activities.com",
                    "discordactivities.com",
                    "discordsays.com",
                    "discordstatus.com",
                    "latency.discord.media",
                    "youtube.com",
                    "googlevideo.com",
                    "ytimg.com",
                    "oaistatic.com",
                    "instagram.com",
                    "cdninstagram.com",
                    "facebook.com",
                    "fbcdn.net",
                    "digitalocean.com"
                ],
                "outboundTag": "proxy",
                "type": "field"
            },
            {
                "network": [
                    "udp"
                ],
                "outboundTag": "proxy",
                "type": "field"
            },
            {
                "ip": [
                    "0.0.0.0/0",
                    "::/0"
                ],
                "outboundTag": "direct",
                "type": "field"
            }
        ]
        }
       ```



</details>
