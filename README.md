# MS SQL Server on Elestio with CI/CD

<a href="https://dash.elest.io/deploy?source=cicd&social=dockerCompose&url=https://github.com/elestio-examples/mssql"><img src="deploy-on-elestio.png" alt="Deploy on Elest.io" width="180px" /></a>

Example CI/CD pipeline showing how to deploy MS SQL Server on Elestio.

# Once deployed ...

You are now able to sign to the SQLPad Web UI here:
    
    https://[CI_CD_DOMAIN]/
    login: sa
    password: [ADMIN_PASSWORD] (set in env var ADMIN_PASSWORD)


You can connect to your instance with Microsoft SQL Server Management Studio

If you don't already have it installed you can download Management Studio here:
https://aka.ms/ssmsfullsetup

    Host: [CI_CD_DOMAIN],18698
    Auth type: SQL Server Authentication
    Login: sa
    Password: Xc[APP_PASSWORD]!2P_G

or with any other tool compatible with MSSQL protocol with those credentials:

Host: [CI_CD_DOMAIN]
Port: 18698
Login: sa
Password: Xc[APP_PASSWORD]!2P_G