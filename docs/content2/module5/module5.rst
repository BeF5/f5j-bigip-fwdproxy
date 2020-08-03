Explicit Proxy用Virtual Server設定
===========================

Explicit Forward Proxyを構成するVirtual Serverを設定します。このVirtual Serverは、クライアントから見たプロキシサーバとして動作します。

**Local Traffic >> Virtual Server** を選択して新規にVirtual Serverを構成し、以下の設定を行います。

- Destination Address/Mask: クライアントのブラウザで指定するIPアドレス、およびサブネットマスク
- Service Port: クライアントのブラウザで指定するポート番号
- HTTP Profile: "HTTP Profile設定"の項で作成したものを指定
- VLAN and Tunnel Traffic: 必要なVLANとトンネルを指定
- Source Address Translation: "Automap"もしくは"SNAT"を指定
- Address Translation: **有効** (チェックを入れる)
- Port Translation: **有効** (チェックを入れる)

  .. figure:: images/mod2-5-1.png
     :scale: 80%
     :align: center

  .. figure:: images/mod2-5-2.png
     :scale: 80%
     :align: center