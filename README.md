# csgo_server

This role installs, updates and configures Counter Strike: Global Offensive dedicated server.

# dependencies

- `hofnarrr.steamcmd`

# example

    - hosts: csgo_servers
      become: yes

      vars:
        csgo_server_rcon_pw: insecure-rcon-password
        csgo_server_gslt: gameserver-login-token
        csgo_server_sv_password: server-password

      roles:
        - hofnarrr.csgo_server
