SSLプロファイル設定
===========================

Explicit Forward Proxyを構成するクライアントおよびサーバSSLプロファイルを設定します。

- **クライアントSSLプロファイル**

  - **Local Traffic >> Profiles >> SSL >> Client** を選択して、クライアントSSLプロファイルを作成します (この例では"clientssl_proxy")。親プロファイル (Parent Profile)として、clientsslを指定します。
  
  .. figure:: images/mod3-2-1.png
     :scale: 80%
     :align: center

　- **SSL Forward Proxy** のセクションで以下の設定を行います。

    - SSL Forward Proxy: **有効** (Enabled)
    - CA Certificate Key Chain: "CA証明書の設定例"の項で作成したCA証明書およびキーを指定
    - SSL Forward Proxy Bypass: **有効** (Enabled)

  .. figure:: images/mod3-2-2.png
     :scale: 80%
     :align: center
  

- **サーバSSLプロファイル**

  - **Local Traffic >> Profiles >> SSL >> Server** を選択して、サーバSSLプロファイルを作成します (この例では"serverssl_proxy")。親プロファイル (Parent Profile)として、serversslを指定します。合わせて、以下の設定を行います。
    
    - SSL Forward Proxy: **有効** (Enabled)
    - SSL Forward Proxy Bypass: **有効** (Enabled)

  .. figure:: images/mod3-2-3.png
     :scale: 80%
     :align: center
  
  - **Server Authentication** のセクションで以下の設定を行います。
    
    - Server Certificate: "require..."を選択
    - Trusted Bundled Authority: "ca-bundle.crt"を選択

  .. figure:: images/mod3-2-4.png
     :scale: 80%
     :align: center


