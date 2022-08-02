<h1 align="center"> Rebus Testnet Rehberi </h1> 

![image](https://user-images.githubusercontent.com/101149671/182340706-3eef17b5-f22c-4239-8867-e9f571ba6cac.png)


<h1 align="center"> Arkadaşlar ödül kısmı yüksek ihtimal sadece 100 kişiye olacak, ona göre karar veriniz, ekibin duyurusu altta: </h1> 

# SORULARINIZ İÇİN KATILIN: [Rebus Türkiye](https://t.me/RebusTurkish)

![image](https://user-images.githubusercontent.com/101149671/182342922-a90ea4a5-9f0f-430b-8dde-ef63bfb0c19e.png)


## Sistem gereksinimleri:
```
4 vCPU
8 RAM (ekibin önerisi 16)
160 SSD
```

## scripti çalıştıralım:
```
wget -q -O rebus.sh https://api.rues.info/rebus.sh && chmod +x rebus.sh && sudo /bin/bash rebus.sh
```

## Loglara bakalım:

* Güvenilir Explorer şu an yok
* sizde bloklar 1-2-3 diye başlar
* Loglar akıyorsa sorun yok faucet bekliycez

```
journalctl -u rebusd -f -o cat
```

![image](https://user-images.githubusercontent.com/101149671/182341600-e28eebca-152a-434a-a98e-734ad6328b17.png)


## Cüzdan oluşturma

* cüzdan ismi değişin

```
rebusd keys add cüzdanismi
```

<h1 align="center"> Şimdi discord kanalına gidip faucet kanalına adres bırakalım, token gelicektir elbet. </h1> 

### [Discord linki](https://discord.gg/uGdygCqr)


## validator oluşturalım. 

* FAUCET AÇILDIĞINDA
```
rebusd tx staking create-validator \
--amount=9900000arebus \
--pubkey=$(rebusd tendermint show-validator) \
--moniker=RuesValidator \
--chain-id=reb_3333-1 \
--commission-rate="0.10" \
--commission-max-rate="0.20" \
--commission-max-change-rate="0.1" \
--min-self-delegation="1" \
--fees=250arebus \
--gas=200000 \
--from=rues \
--website="http://forum.rues.info/" \
--details="https://linktr.ee/ruesandora0" \
-y
```
# SORULARINIZ İÇİN: [Rebus Türkiye](https://t.me/RebusTurkish)

# Hesaplar:

[<img src="https://cdn-icons-png.flaticon.com/512/733/733579.png" width="16px"> Twitter   ](https://twitter.com/Ruesandora0) 

[<img src="https://cdn-icons-png.flaticon.com/512/1336/1336494.png" width="16px"> Forum   ](https://forum.rues.info/index.php)

[<img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" width="16px"> Telegram Announcement   ](https://t.me/RuesAnnouncement)

[<img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" width="16px"> Telegram Chat   ](https://t.me/+-l6GpqiNOxFiMTVk)

[Discord](https://discord.gg/ruescommunity)
