トンネル用Virtual Server設定
===========================

HTTPS通信においてトンネルを構成するVirtual Serverを設定します。

**Local Traffic >> Virtual Server** を選択して新規にVirtual Serverを構成し、以下の設定を行います。

- Destination Address/Mask: "0.0.0.0/0"を指定
- Service Port: 通常は"443" (HTTPS)を指定
- SSL Profile (Client): "SSLプロファイル設定"の項で作成したClient SSL Profileを指定
- SSL Profile (Server): "SSLプロファイル設定"の項で作成したServer SSL Profileを指定
- Source Address Translation: "Automap"もしくは"SNAT"を指定
- Address Translation: **無効** (チェックを外す)
- Port Translation: **無効** (チェックを外す)


  .. figure:: images/mod3-3-1.png
     :scale: 60%
     :align: center

  .. figure:: images/mod3-3-2.png
     :scale: 60%
     :align: center

  .. figure:: images/mod3-3-3.png
     :scale: 80%
     :align: center
