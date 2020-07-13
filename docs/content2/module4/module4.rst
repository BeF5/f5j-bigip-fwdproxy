HTTPプロファイル設定
===========================

Explicit Forward Proxyを構成するHTTPプロファイルを設定します。

**Local Traffic >> Profiles >> Services** を選択して、HTTPプロファイルを作成します。

- **General Properties** のセクションで以下の設定を行います。

  - Proxy Mode: "Explicit"を選択
  - Parent Profile: "http-explicit"を選択

  .. figure:: images/mod2-4-1.png
     :scale: 80%
     :align: center

 - **Explicit Proxy** のセクションで以下の設定を行います。

  - DNS Resolver: "DNSリゾルバの設定"の項で作成したものを選択します。
  - Tunnel Names: "TLSをサポートするTCPトンネルの設定"の項で作成したものを選択します。

  .. figure:: images/mod2-4-2.png
     :scale: 60%
     :align: center


   