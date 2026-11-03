# 3x-ui 汉化管理脚本 · 中英对照表

适用于 [wantaiyu1/3-x-ui `zh-cn`](https://github.com/wantaiyu1/3-x-ui/tree/zh-cn) 分支的
`x-ui.sh`（管理菜单）、`install.sh`（安装脚本）、`update.sh`（更新脚本）。

共 **856** 条对照。命令名（`x-ui start` 等子命令）、路径、`${变量}`、服务名、sysctl 键、fail2ban 正则等按原样保留。
`${...}` 是脚本内的变量占位，运行时会被替换成实际值。

| # | 英文原文 | 中文译文 |
|---|---|---|
| 1 | `10-xui-sandbox.conf: $whitespace_paths` | 10-xui-sandbox.conf 之外：$whitespace_paths |
| 2 | `The panel cannot write to them under the unit's sandbox.` | 在 unit 沙箱下，面板无法写入这些目录。 |
| 3 | `The panel's folders stay writable through ReadWriteDirectories=, the alias this script installs.` | 面板的目录通过本脚本安装的 ReadWriteDirectories= 别名保持可写。 |
| 4 | `Not applied, needs a newer systemd: ${missing}.` | 未应用，需要更新版本的 systemd：${missing}。 |
| 5 | `The panel's folders stay writable through ReadWriteDirectories=, the alias this script installs.` | 面板的目录通过本脚本安装的 ReadWriteDirectories= 别名保持可写。 |
| 6 | `The rest of the hardening is in force. Upgrade systemd to apply the above.` | 其余加固配置已生效。升级 systemd 后可应用上述配置。 |
| 7 | `docker restart <container_name>` | docker restart <容器名> |
| 8 | `docker stop <container_name>` | docker stop <容器名> |
| 9 | `${blue}sudo -u postgres psql -d ${PG_DB}${plain} (as the postgres superuser)` | ${blue}sudo -u postgres psql -d ${PG_DB}${plain} （以 postgres 超级用户身份） |
| 10 | `- Certificate File: $webCertFile` | - 证书文件：$webCertFile |
| 11 | `- Private Key File: $webKeyFile` | - 私钥文件：$webKeyFile |
| 12 | `- Validity: ~6 days (auto-renews via acme.sh cron)` | - 有效期：约 6 天（由 acme.sh 定时任务自动续期） |
| 13 | `1) Install PostgreSQL locally and create a dedicated user/db (recommended)` | 1) 本机安装 PostgreSQL 并创建专用用户/数据库（推荐） |
| 14 | `1) Retry local install` | 1) 重试本机安装 |
| 15 | `1) SQLite (default — recommended for < 500 clients)` | 1) SQLite （默认 — 客户端少于 500 时推荐） |
| 16 | `2) Enter an external DSN instead` | 2) 改为输入外部 DSN |
| 17 | `2) PostgreSQL (recommended for high client counts / many nodes)` | 2) PostgreSQL （客户端数量多 / 节点多时推荐） |
| 18 | `2) Use an existing PostgreSQL server (enter DSN)` | 2) 使用已有的 PostgreSQL 服务器（输入 DSN） |
| 19 | `3) Abort install` | 3) 中止安装 |
| 20 | `4) Fall back to SQLite` | 4) 回退使用 SQLite |
| 21 | `Cert: ${certDir}/fullchain.pem` | 证书：${certDir}/fullchain.pem |
| 22 | `If using an SSH key:` | 如使用 SSH 密钥： |
| 23 | `Key: ${certDir}/privkey.pem` | 私钥：${certDir}/privkey.pem |
| 24 | `Standard SSH command:` | 标准 SSH 命令： |
| 25 | `Then open in your browser:` | 然后在浏览器中打开： |
| 26 | `docker restart <container_name>` | docker restart <容器名> |
| 27 | `docker stop <container_name>` | docker stop <容器名> |
| 28 | `of the first configured cluster on Debian-style installs (e.g.` | （Debian 系安装时指首个已配置集群的），例如 |
| 29 | `# Added by 3x-ui: allow password logins for the panel database.` | # 由 3x-ui 添加：允许面板数据库使用密码登录。 |
| 30 | `${blue} (as the postgres superuser)${plain}` | ${blue} （以 postgres 超级用户身份执行）${plain} |
| 31 | `${blue}Note:${plain} Option 4 serves the panel over plain HTTP — only safe behind nginx/Caddy or an SSH tunnel.` | ${blue}注意：${plain} 选项 4 会让面板以纯 HTTP 提供服务 — 仅在 nginx/Caddy 或 SSH 隧道之后才安全。 |
| 32 | `${blue}Note:${plain} Options 1 & 2 require port 80 open. Option 3 requires manual paths.` | ${blue}注意：${plain} 选项 1 和 2 需要开放 80 端口，选项 3 需手动指定路径。 |
| 33 | `${dat}.dat: already up to date` | ${dat}.dat：已是最新版本 |
| 34 | `${green} Database Selection ${plain}` | ${green} 数据库选择 ${plain} |
| 35 | `${green} Panel Access Information ${plain}` | ${green} 面板访问信息 ${plain} |
| 36 | `${green} Panel Installation Complete! ${plain}` | ${green} 面板安装完成！ ${plain} |
| 37 | `${green} PostgreSQL Credentials ${plain}` | ${green} PostgreSQL 凭据 ${plain} |
| 38 | `${green} SSL Certificate Setup (RECOMMENDED) ${plain}` | ${green} SSL 证书设置（推荐） ${plain} |
| 39 | `${green} 2.${plain} Input your own command` | ${green} 2.${plain} 手动输入自定义命令 |
| 40 | `${green} Please use the new login username and password to access the X-UI panel. Also remember them! ${plain}` | ${green} 请使用新的用户名和密码登录 X-UI 面板，并务必牢记！${plain} |
| 41 | `${green}${name} are already up to date, restart is not needed.${plain}` | ${green}${name} 已是最新版本，无需重启。${plain} |
| 42 | `${green}${name} have been updated successfully!${plain}` | ${green}${name} 已更新成功！${plain} |
| 43 | `${green}0.${plain} Back to Main Menu` | ${green}0.${plain} 返回主菜单 |
| 44 | `${green}1.${plain} Let's Encrypt for Domain (90-day validity, auto-renews)` | ${green}1.${plain} 为域名申请 Let's Encrypt 证书（90 天有效，自动续期） |
| 45 | `${green}1.${plain} Set listen IP` | ${green}1.${plain} 设置监听 IP |
| 46 | `${green}2.${plain} Clear listen IP` | ${green}2.${plain} 清除监听 IP |
| 47 | `${green}2.${plain} Let's Encrypt for IP Address (6-day validity, auto-renews)` | ${green}2.${plain} 为 IP 地址申请 Let's Encrypt 证书（6 天有效，自动续期） |
| 48 | `${green}3.${plain} Custom SSL Certificate (Path to existing files)` | ${green}3.${plain} 自定义 SSL 证书（指定现有文件路径） |
| 49 | `${green}3X-IPL ban log entries:${plain}` | ${green}3X-IPL 封禁日志条目：${plain} |
| 50 | `${green}4.${plain} Skip SSL (advanced — behind reverse proxy / SSH tunnel only)` | ${green}4.${plain} 跳过 SSL（高级用法 — 仅限反向代理 / SSH 隧道场景） |
| 51 | `${green}API Token: ${config_apiToken}${plain}` | ${green}API 令牌： ${config_apiToken}${plain} |
| 52 | `${green}Access URL: ${SSL_SCHEME}://${SSL_HOST}:${config_port}/${config_webBasePath}${plain}` | ${green}访问地址： ${SSL_SCHEME}://${SSL_HOST}:${config_port}/${config_webBasePath}${plain} |
| 53 | `${green}Access URL: ${SSL_SCHEME}://${SSL_HOST}:${existing_port}/${config_webBasePath}${plain}` | ${green}访问地址： ${SSL_SCHEME}://${SSL_HOST}:${existing_port}/${config_webBasePath}${plain} |
| 54 | `${green}Access URL: ${SSL_SCHEME}://${SSL_HOST}:${existing_port}/${existing_webBasePath}${plain}` | ${green}访问地址： ${SSL_SCHEME}://${SSL_HOST}:${existing_port}/${existing_webBasePath}${plain} |
| 55 | `${green}Access URL: ${access_scheme}://${access_host}:${existing_port}/${existing_webBasePath}${plain}` | ${green}访问地址：${access_scheme}://${access_host}:${existing_port}/${existing_webBasePath}${plain} |
| 56 | `${green}Access URL: https://${CF_Domain}:${existing_port}${existing_webBasePath}${plain}` | ${green}访问地址：https://${CF_Domain}:${existing_port}${existing_webBasePath}${plain} |
| 57 | `${green}Access URL: https://${domain}:${existing_port}${existing_webBasePath}${plain}` | ${green}访问地址：https://${domain}:${existing_port}${existing_webBasePath}${plain} |
| 58 | `${green}Access URL: https://${domain}:${existing_port}/${existing_webBasePath}${plain}` | ${green}访问地址：https://${domain}:${existing_port}/${existing_webBasePath}${plain} |
| 59 | `${green}Access URL: https://${server_ip}:${existing_port}${existing_webBasePath}${plain}` | ${green}访问地址：https://${server_ip}:${existing_port}${existing_webBasePath}${plain} |
| 60 | `${green}Access URL: https://${server_ip}:${existing_port}/${config_webBasePath}${plain}` | ${green}访问地址：https://${server_ip}:${existing_port}/${config_webBasePath}${plain} |
| 61 | `${green}Added x-ui.db to /etc/.gitignore for etckeeper${plain}` | ${green}已将 x-ui.db 添加到 /etc/.gitignore（供 etckeeper 使用）${plain} |
| 62 | `${green}All users Unbanned successfully.${plain}` | ${green}所有用户已成功解封。${plain} |
| 63 | `${green}Auto renew succeeded, certificate details:${plain}` | ${green}自动续期设置成功，证书详情：${plain} |
| 64 | `${green}BBR has been enabled successfully.${plain}` | ${green}BBR 已成功开启。${plain} |
| 65 | `${green}BBR has been replaced with CUBIC successfully.${plain}` | ${green}已成功将 BBR 替换为 CUBIC。${plain} |
| 66 | `${green}BBR is already enabled!${plain}` | ${green}BBR 已处于开启状态！${plain} |
| 67 | `${green}Certificate File: $webCertFile${plain}` | ${green}证书文件：$webCertFile${plain} |
| 68 | `${green}Certificate files installed successfully${plain}` | ${green}证书文件安装成功${plain} |
| 69 | `${green}Certificate issued successfully, installing...${plain}` | ${green}证书申请成功，正在安装...${plain} |
| 70 | `${green}Certificate paths configured successfully${plain}` | ${green}证书路径配置成功${plain} |
| 71 | `${green}Certificate paths set for the panel${plain}` | ${green}面板证书路径已设置${plain} |
| 72 | `${green}Certificate valid for ~6 days, auto-renews via acme.sh cron job.${plain}` | ${green}证书有效期约 6 天，由 acme.sh 定时任务自动续期。${plain} |
| 73 | `${green}Changing on config file permissions...${plain}` | ${green}正在修改配置文件权限...${plain} |
| 74 | `${green}Changing owner...${plain}` | ${green}正在修改所有者...${plain} |
| 75 | `${green}Checking ban logs...${plain}` | ${green}正在检查封禁日志...${plain} |
| 76 | `${green}Checksum verified: ${actual_sha256}${plain}` | ${green}校验通过：${actual_sha256}${plain} |
| 77 | `${green}Checksum verified: ${actual}${plain}` | ${green}校验通过：${actual}${plain} |
| 78 | `${green}Configuring IP Limit...${plain}` | ${green}正在配置 IP 限制...${plain} |
| 79 | `${green}Connect from this server:${plain}` | ${green}从本服务器连接：${plain} |
| 80 | `${green}Connection DSN:${plain} ${dsn}` | ${green}连接 DSN：${plain} ${dsn} |
| 81 | `${green}Created /etc/.gitignore and added x-ui.db for etckeeper${plain}` | ${green}已创建 /etc/.gitignore 并添加 x-ui.db（供 etckeeper 使用）${plain} |
| 82 | `${green}Current SSH Port Forwarding Configuration:${plain}` | ${green}当前 SSH 端口转发配置：${plain} |
| 83 | `${green}Current listen IP is already set to ${config_listenIP}.${plain}` | ${green}当前监听 IP 已设置为 ${config_listenIP}。${plain} |
| 84 | `${green}Current x-ui version: ${current_xui_version}${plain}` | ${green}当前 x-ui 版本：${current_xui_version}${plain} |
| 85 | `${green}DB Name: ${PG_DB}${plain}` | ${green}数据库名： ${PG_DB}${plain} |
| 86 | `${green}DSN: ${xui_dsn}${plain}` | ${green}DSN： ${xui_dsn}${plain} |
| 87 | `${green}Database: ${db_label}${plain}` | ${green}数据库： ${db_label}${plain} |
| 88 | `${green}Database: SQLite (/etc/x-ui/x-ui.db)${plain}` | ${green}数据库：SQLite (/etc/x-ui/x-ui.db)${plain} |
| 89 | `${green}Default --reloadcmd for ACME is: ${yellow}systemctl restart x-ui \|\| rc-service x-ui restart${plain}` | ${green}ACME 默认 --reloadcmd 为：${yellow}systemctl restart x-ui \|\| rc-service x-ui restart${plain} |
| 90 | `${green}Downloading new x-ui version...${plain}` | ${green}正在下载新版本 x-ui...${plain} |
| 91 | `${green}Downloading startup unit x-ui.rc...${plain}` | ${green}正在下载启动单元 x-ui.rc...${plain} |
| 92 | `${green}Env file: ${xui_env_file}${plain}` | ${green}环境文件： ${xui_env_file}${plain} |
| 93 | `${green}Fail2ban and IP Limit removed successfully!${plain}` | ${green}Fail2ban 与 IP 限制已成功移除！${plain} |
| 94 | `${green}Fail2ban installed successfully!${plain}` | ${green}Fail2ban 安装成功！${plain} |
| 95 | `${green}Fail2ban is not installed. Installing now...!${plain}` | ${green}未安装 Fail2ban，正在安装...！${plain} |
| 96 | `${green}Fail2ban setup complete.${plain}` | ${green}Fail2ban 配置完成。${plain} |
| 97 | `${green}Found x-ui.service in extracted files, installing...${plain}` | ${green}在解压文件中找到 x-ui.service，正在安装...${plain} |
| 98 | `${green}Found x-ui.service.arch in extracted files, installing...${plain}` | ${green}在解压文件中找到 x-ui.service.arch，正在安装...${plain} |
| 99 | `${green}Found x-ui.service.debian in extracted files, installing...${plain}` | ${green}在解压文件中找到 x-ui.service.debian，正在安装...${plain} |
| 100 | `${green}Found x-ui.service.rhel in extracted files, installing...${plain}` | ${green}在解压文件中找到 x-ui.service.rhel，正在安装...${plain} |
| 101 | `${green}Host: ${PG_HOST}${plain}` | ${green}主机： ${PG_HOST}${plain} |
| 102 | `${green}IP Address ${ban_ip} has been banned successfully.${plain}` | ${green}IP 地址 ${ban_ip} 已成功封禁。${plain} |
| 103 | `${green}IP Address ${unban_ip} has been unbanned successfully.${plain}` | ${green}IP 地址 ${unban_ip} 已成功解封。${plain} |
| 104 | `${green}IP Limit installed and configured successfully!${plain}` | ${green}IP 限制安装并配置成功！${plain} |
| 105 | `${green}IP Limit removed successfully!${plain}` | ${green}IP 限制已成功移除！${plain} |
| 106 | `${green}IP certificate installed and configured successfully!${plain}` | ${green}IP 证书已成功安装并配置！${plain} |
| 107 | `${green}Including IPv6 address: ${ipv6}${plain}` | ${green}包含 IPv6 地址：${ipv6}${plain} |
| 108 | `${green}Install result written to ${result_file} (mode 600).${plain}` | ${green}安装结果已写入 ${result_file}（权限 600）。${plain} |
| 109 | `${green}Installing acme.sh for SSL certificate management...${plain}` | ${green}正在安装 acme.sh 用于 SSL 证书管理...${plain} |
| 110 | `${green}Installing arch-like systemd unit...${plain}` | ${green}正在安装 Arch 系 systemd unit...${plain} |
| 111 | `${green}Installing certificate succeeded, enabling auto renew...${plain}` | ${green}证书安装成功，正在启用自动续期...${plain} |
| 112 | `${green}Installing debian-like systemd unit...${plain}` | ${green}正在安装 Debian 系 systemd unit...${plain} |
| 113 | `${green}Installing new x-ui version...${plain}` | ${green}正在安装新版 x-ui...${plain} |
| 114 | `${green}Installing rhel-like systemd unit...${plain}` | ${green}正在安装 RHEL 系 systemd unit...${plain} |
| 115 | `${green}Installing startup unit x-ui.rc...${plain}` | ${green}正在安装启动单元 x-ui.rc...${plain} |
| 116 | `${green}Installing systemd unit...${plain}` | ${green}正在安装 systemd unit...${plain} |
| 117 | `${green}Installing x-ui.sh script...${plain}` | ${green}正在安装 x-ui.sh 脚本...${plain} |
| 118 | `${green}Ip Limit jail files created with a bantime of ${bantime} minutes.${plain}` | ${green}已创建 IP 限制 jail 文件，封禁时长 ${bantime} 分钟。${plain} |
| 119 | `${green}Issuing IP certificate for ${ipv4}...${plain}` | ${green}正在为 ${ipv4} 申请 IP 证书...${plain} |
| 120 | `${green}Issuing SSL certificate for ${domain}...${plain}` | ${green}正在为 ${domain} 申请 SSL 证书...${plain} |
| 121 | `${green}Issuing certificate succeeded, installing certificates...${plain}` | ${green}证书签发成功，正在安装证书...${plain} |
| 122 | `${green}Keeping default reloadcmd${plain}` | ${green}保持默认 reloadcmd${plain} |
| 123 | `${green}Listen IP has been cleared.${plain}` | ${green}监听 IP 已清除。${plain} |
| 124 | `${green}Migrating database...${plain}` | ${green}正在迁移数据库...${plain} |
| 125 | `${green}New WebBasePath: ${config_webBasePath}${plain}` | ${green}新的 WebBasePath：${config_webBasePath}${plain} |
| 126 | `${green}Panel is secure with SSL.${plain}` | ${green}面板已启用 SSL，连接安全。${plain} |
| 127 | `${green}Password: ${config_password}${plain}` | ${green}密码： ${config_password}${plain} |
| 128 | `${green}Password: ${PG_PASS}${plain}` | ${green}密码： ${PG_PASS}${plain} |
| 129 | `${green}Please use the new web base path to access the panel.${plain}` | ${green}请使用新的 Web 根路径访问面板。${plain} |
| 130 | `${green}Port ${WebPort} is free and ready for standalone validation.${plain}` | ${green}端口 ${WebPort} 空闲，可用于独立验证。${plain} |
| 131 | `${green}Port: ${config_port}${plain}` | ${green}端口： ${config_port}${plain} |
| 132 | `${green}Port: ${PG_PORT}${plain}` | ${green}端口： ${PG_PORT}${plain} |
| 133 | `${green}PostgreSQL backup & restore is built into the panel:${plain}` | ${green}PostgreSQL 备份与恢复已内置于面板：${plain} |
| 134 | `${green}PostgreSQL is listening on port 5432:${plain}` | ${green}PostgreSQL 正在监听端口 5432：${plain} |
| 135 | `${green}Private Key File: $webKeyFile${plain}` | ${green}私钥文件：$webKeyFile${plain} |
| 136 | `${green}Recent system ban activities from fail2ban.log:${plain}` | ${green}fail2ban.log 中最近的系统封禁记录：${plain} |
| 137 | `${green}Reloadcmd is: ${reloadCmd}${plain}` | ${green}reloadcmd 为：${reloadCmd}${plain} |
| 138 | `${green}Reloadcmd is: systemctl reload nginx ; systemctl restart x-ui${plain}` | ${green}reloadcmd 为：systemctl reload nginx ; systemctl restart x-ui${plain} |
| 139 | `${green}Removing old README and LICENSE file...${plain}` | ${green}正在移除旧的 README 与 LICENSE 文件...${plain} |
| 140 | `${green}Removing old mtg version...${plain}` | ${green}正在移除旧版 mtg...${plain} |
| 141 | `${green}Removing old service unit version...${plain}` | ${green}正在移除旧的服务单元...${plain} |
| 142 | `${green}Removing old systemd unit version...${plain}` | ${green}正在移除旧的 systemd unit...${plain} |
| 143 | `${green}Removing old x-ui version...${plain}` | ${green}正在移除旧版 x-ui...${plain} |
| 144 | `${green}Removing old xray version...${plain}` | ${green}正在移除旧版 xray...${plain} |
| 145 | `${green}Restored custom file(s) in bin/ not shipped by this release: ${restored_custom_bin[*]}${plain}` | ${green}已恢复 bin/ 中本版本未提供的自定义文件：${restored_custom_bin[*]}${plain} |
| 146 | `${green}SSH Port Forwarding Configuration:${plain}` | ${green}SSH 端口转发配置：${plain} |
| 147 | `${green}SSH Port Forwarding — open the panel from your local machine via:${plain}` | ${green}SSH 端口转发 — 在本地机器上通过以下方式打开面板：${plain} |
| 148 | `${green}SSH 端口转发 — 在本地机器上通过以下方式打开面板：${plain}` | ${green}SSH 端口转发 —— 请在本地机器上执行以下命令打开面板：${plain} |
| 149 | `${green}SSL certificate already configured. No action needed.${plain}` | ${green}SSL 证书已配置，无需操作。${plain} |
| 150 | `${green}SSL certificate installed and configured successfully!${plain}` | ${green}SSL 证书已成功安装并配置！${plain} |
| 151 | `${green}Setting certificate paths for the panel...${plain}` | ${green}正在为面板设置证书路径...${plain} |
| 152 | `${green}Setting up Fail2ban for the IP Limit feature...${plain}` | ${green}正在为 IP 限制功能配置 Fail2ban...${plain} |
| 153 | `${green}Setting up Let's Encrypt IP certificate (shortlived profile)...${plain}` | ${green}正在申请 Let's Encrypt IP 证书（shortlived 配置）...${plain} |
| 154 | `${green}Setting up SSL certificate...${plain}` | ${green}正在配置 SSL 证书...${plain} |
| 155 | `${green}Setting up systemd unit...${plain}` | ${green}正在配置 systemd unit...${plain} |
| 156 | `${green}Stopping x-ui...${plain}` | ${green}正在停止 x-ui...${plain} |
| 157 | `${green}This command will run on every certificate issue and renew.${plain}` | ${green}该命令将在每次签发和续期证书时执行。${plain} |
| 158 | `${green}Unsupported CPU architecture! ${plain}` | ${green}不支持的 CPU 架构！${plain} |
| 159 | `${green}Update successful. The panel has automatically restarted.${plain}` | ${green}更新成功，面板已自动重启。${plain} |
| 160 | `${green}Updating and install dependency packages...${plain}` | ${green}正在更新并安装依赖包...${plain} |
| 161 | `${green}Username, Password, and WebBasePath are properly set.${plain}` | ${green}用户名、密码和 WebBasePath 均已正确设置。${plain} |
| 162 | `${green}Username: ${config_username}${plain}` | ${green}用户名： ${config_username}${plain} |
| 163 | `${green}Username: ${PG_USER}${plain}` | ${green}用户名： ${PG_USER}${plain} |
| 164 | `${green}Using Let's Encrypt for IP certificate (shortlived profile)...${plain}` | ${green}正在使用 Let's Encrypt 申请 IP 证书（shortlived 配置）...${plain} |
| 165 | `${green}Using Let's Encrypt for domain certificate...${plain}` | ${green}正在使用 Let's Encrypt 申请域名证书...${plain} |
| 166 | `${green}Using custom existing certificate...${plain}` | ${green}正在使用已有的自定义证书...${plain} |
| 167 | `${green}Using existing certificate, installing certificates...${plain}` | ${green}使用已有证书，正在安装证书...${plain} |
| 168 | `${green}Using port ${WebPort} for standalone validation.${plain}` | ${green}使用端口 ${WebPort} 进行独立验证。${plain} |
| 169 | `${green}Using update tag: ${tag_version}${plain}` | ${green}使用更新标签：${tag_version}${plain} |
| 170 | `${green}WebBasePath: ${config_webBasePath}${plain}` | ${green}Web 跟路径：${config_webBasePath}${plain} |
| 171 | `${green}Will use port: ${WebPort} to issue certificates. Please make sure this port is open.${plain}` | ${green}将使用端口 ${WebPort} 签发证书，请确保该端口已开放。${plain} |
| 172 | `${green}Your domain is ready for issuing certificates now...${plain}` | ${green}您的域名已就绪，可以签发证书了...${plain} |
| 173 | `${green}Your domain is: ${domain}, checking it...${plain}` | ${green}您的域名是：${domain}，正在检查...${plain} |
| 174 | `${green}\ 0.${plain} Back to Main Menu` | ${green}\ 0.${plain} 返回主菜单 |
| 175 | `${green}\ 1.${plain} Loyalsoldier (geoip.dat, geosite.dat)` | ${green}\ 1.${plain} Loyalsoldier（geoip.dat、geosite.dat） |
| 176 | `${green}\ 4.${plain} ${red}Delete${plain} Ports from List` | ${green}\ 4.${plain} ${red}删除${plain}列表中的端口 |
| 177 | `${green} 0.${plain} Back to Main Menu` | ${green} 0.${plain} 返回主菜单 |
| 178 | `${green} 1.${plain} ${green}Install${plain} Firewall` | ${green} 1.${plain} ${green}安装${plain}防火墙 |
| 179 | `${green} 1.${plain} ${green}Install${plain} PostgreSQL (server + client + xui db)` | ${green} 1.${plain} ${green}安装${plain} PostgreSQL（服务端 + 客户端 + xui 数据库） |
| 180 | `${green} 1.${plain} Debug Log` | ${green} 1.${plain} 调试日志 |
| 181 | `${green} 1.${plain} Enable BBR` | ${green} 1.${plain} 开启 BBR |
| 182 | `${green} 1.${plain} Get SSL (Domain)` | ${green} 1.${plain} 申请 SSL 证书（域名） |
| 183 | `${green} 1.${plain} Install PostgreSQL locally and create a dedicated user/db (recommended)` | ${green} 1.${plain} 本机安装 PostgreSQL 并创建专用用户/数据库（推荐） |
| 184 | `${green} 1.${plain} Only remove IP Limit configurations` | ${green} 1.${plain} 仅移除 IP 限制配置 |
| 185 | `${green} 1.${plain} Use a certificate from /root/cert` | ${green} 1.${plain} 使用 /root/cert 中的证书 |
| 186 | `${green} 10.${plain} Install/Upgrade client tools (pg_dump/pg_restore)` | ${green} 10.${plain} 安装/升级客户端工具（pg_dump/pg_restore） |
| 187 | `${green} 10.${plain} Uninstall Fail2ban and IP Limit` | ${green} 10.${plain} 卸载 Fail2ban 与 IP 限制 |
| 188 | `${green} 2.${plain} Change Ban Duration` | ${green} 2.${plain} 修改封禁时长 |
| 189 | `${green} 2.${plain} Clear All logs` | ${green} 2.${plain} 清空所有日志 |
| 190 | `${green} 2.${plain} Disable BBR` | ${green} 2.${plain} 关闭 BBR |
| 191 | `${green} 2.${plain} Enter custom certificate file paths (e.g. certbot, /etc/letsencrypt/...)` | ${green} 2.${plain} 手动输入证书文件路径（例如 certbot、/etc/letsencrypt/...） |
| 192 | `${green} 2.${plain} Migrate SQLite ${green}->${plain} PostgreSQL` | ${green} 2.${plain} 迁移 SQLite ${green}->${plain} PostgreSQL |
| 193 | `${green} 2.${plain} Port List [numbered]` | ${green} 2.${plain} 端口列表 [带编号] |
| 194 | `${green} 2.${plain} Revoke & Remove` | ${green} 2.${plain} 吊销并删除证书 |
| 195 | `${green} 2.${plain} Uninstall Fail2ban and IP Limit` | ${green} 2.${plain} 卸载 Fail2ban 与 IP 限制 |
| 196 | `${green} 2.${plain} Use an existing PostgreSQL server (enter DSN)` | ${green} 2.${plain} 使用已有的 PostgreSQL 服务器（输入 DSN） |
| 197 | `${green} 3.${plain} ${green}Open${plain} Ports` | ${green} 3.${plain} ${green}开放${plain}端口 |
| 198 | `${green} 3.${plain} Force Renew` | ${green} 3.${plain} 强制续期 |
| 199 | `${green} 3.${plain} Status (clusters & port 5432)` | ${green} 3.${plain} 状态（集群与 5432 端口） |
| 200 | `${green} 3.${plain} Unban Everyone` | ${green} 3.${plain} 解封所有 IP |
| 201 | `${green} 4.${plain} ${red}Delete${plain} Ports from List` | ${green} 4.${plain} ${red}删除${plain}列表中的端口 |
| 202 | `${green} 4.${plain} All` | ${green} 4.${plain} 全部 |
| 203 | `${green} 4.${plain} Ban Logs` | ${green} 4.${plain} 封禁日志 |
| 204 | `${green} 4.${plain} Show Existing Domains` | ${green} 4.${plain} 查看已有域名 |
| 205 | `${green} 5.${plain} ${green}Enable${plain} Firewall` | ${green} 5.${plain} ${green}启用${plain}防火墙 |
| 206 | `${green} 5.${plain} Ban an IP Address` | ${green} 5.${plain} 封禁指定 IP |
| 207 | `${green} 5.${plain} Set Cert paths for the panel` | ${green} 5.${plain} 为面板设置证书路径 |
| 208 | `${green} 6.${plain} ${red}Disable${plain} Firewall` | ${green} 6.${plain} ${red}禁用${plain}防火墙 |
| 209 | `${green} 6.${plain} Get SSL for IP Address (6-day cert, auto-renews)` | ${green} 6.${plain} 为 IP 地址申请 SSL 证书（6 天有效，自动续期） |
| 210 | `${green} 6.${plain} Restart PostgreSQL` | ${green} 6.${plain} 重启 PostgreSQL |
| 211 | `${green} 6.${plain} Unban an IP Address` | ${green} 6.${plain} 解封指定 IP |
| 212 | `${green} 7.${plain} ${green}Enable${plain} Autostart on boot` | ${green} 7.${plain} ${green}开启${plain}开机自启 |
| 213 | `${green} 7.${plain} Firewall Status` | ${green} 7.${plain} 防火墙状态 |
| 214 | `${green} 7.${plain} Real-Time Logs` | ${green} 7.${plain} 实时日志 |
| 215 | `${green} 8.${plain} Service Status` | ${green} 8.${plain} 服务状态 |
| 216 | `${green} 8.${plain} View PostgreSQL Log` | ${green} 8.${plain} 查看 PostgreSQL 日志 |
| 217 | `${green} 9.${plain} Convert SQLite ${green}.db <-> .dump${plain}` | ${green} 9.${plain} 转换 SQLite ${green}.db <-> .dump${plain} |
| 218 | `${green} 9.${plain} Service Restart` | ${green} 9.${plain} 重启服务 |
| 219 | `${green}\u2713 Custom certificate paths applied.${plain}` | ${green}\u2713 自定义证书路径已应用。${plain} |
| 220 | `${green}\u2713 Let's Encrypt IP certificate configured successfully${plain}` | ${green}\u2713 Let's Encrypt IP 证书配置成功${plain} |
| 221 | `${green}\u2713 Panel bound to 127.0.0.1 only. It is now unreachable from the public internet.${plain}` | ${green}\u2713 面板已仅绑定到 127.0.0.1，现无法从公网访问。${plain} |
| 222 | `${green}\u2713 SSL certificate configured successfully with domain: ${cert_domain}${plain}` | ${green}\u2713 已成功为域名 ${cert_domain} 配置 SSL 证书${plain} |
| 223 | `${green}\u2713 SSL setup skipped.${plain}` | ${green}\u2713 已跳过 SSL 配置。${plain} |
| 224 | `${green}acme.sh installed successfully${plain}` | ${green}acme.sh 安装成功${plain} |
| 225 | `${green}listen IP has been set to ${config_listenIP}.${plain}` | ${green}监听 IP 已设置为 ${config_listenIP}。${plain} |
| 226 | `${green}x-ui ${tag_version}${plain} installation finished, it is running now...` | ${green}x-ui ${tag_version}${plain} 安装完成，现已运行... |
| 227 | `${green}x-ui ${tag_version}${plain} updating finished, it is running now...` | ${green}x-ui ${tag_version}${plain} 更新完成，现已运行... |
| 228 | `${green}✓ Custom certificate paths applied.${plain}` | ${green}✓ 已应用自定义证书路径。${plain} |
| 229 | `${green}✓ Let\'s Encrypt IP certificate configured successfully${plain}` | ${green}✓ Let\'s Encrypt IP 证书配置成功${plain} |
| 230 | `${green}✓ Panel bound to 127.0.0.1 only. It is now unreachable from the public internet.${plain}` | ${green}✓ 面板仅监听 127.0.0.1，公网已无法访问。${plain} |
| 231 | `${green}✓ SSL certificate configured successfully with domain: ${cert_domain}${plain}` | ${green}✓ SSL 证书已配置成功，域名：${cert_domain}${plain} |
| 232 | `${green}✓ SSL setup skipped.${plain}` | ${green}✓ 已跳过 SSL 设置。${plain} |
| 233 | `${red}${NUM} is not a number! Please, try again.${plain}` | ${red}${NUM} 不是数字！请重新输入。${plain} |
| 234 | `${red}${dat}.dat: download failed${plain}` | ${red}${dat}.dat：下载失败${plain} |
| 235 | `${red}${dat}.dat: downloaded file is empty${plain}` | ${red}${dat}.dat：下载的文件为空${plain} |
| 236 | `${red}${dat}.dat: failed to install${plain}` | ${red}${dat}.dat：安装失败${plain} |
| 237 | `${red}${name} is not available for ${ref} (HTTP ${status})${plain}` | ${red}${name} 在 ${ref} 中不可用（HTTP ${status}）${plain} |
| 238 | `${red}Any existing panel tables in the destination will be cleared and overwritten.${plain}` | ${red}目标库中已有的面板数据表将被清空并覆盖。${plain} |
| 239 | `${red}Ban log file not found at: ${iplimit_banned_log_path}${plain}` | ${red}未找到封禁日志文件：${iplimit_banned_log_path}${plain} |
| 240 | `${red}Certificate files not found after installation${plain}` | ${red}安装后未找到证书文件${plain} |
| 241 | `${red}Checksum mismatch for $(basename` | ${red}校验和不匹配：$(basename |
| 242 | `${red}Checksum mismatch for $(basename "${file}"): expected ${expected:-<none>}, got ${actual}${plain}` | ${red}$(basename "${file}") 校验值不匹配：期望 ${expected:-<none>}，实际 ${actual}${plain} |
| 243 | `${red}Domain name cannot be empty. Please try again.${plain}` | ${red}域名不能为空，请重新输入。${plain} |
| 244 | `${red}Download x-ui ${tag_version} failed, please check if the version exists ${plain}` | ${red}下载 x-ui ${tag_version} 失败，请检查该版本是否存在 ${plain} |
| 245 | `${red}Downloaded x-ui release archive is empty${plain}` | ${red}下载的 x-ui 发布压缩包为空${plain} |
| 246 | `${red}Downloaded x-ui.rc is empty${plain}` | ${red}下载的 x-ui.rc 为空${plain} |
| 247 | `${red}Downloaded x-ui.sh is empty${plain}` | ${red}下载的 x-ui.sh 为空${plain} |
| 248 | `${red}Downloading x-ui failed, please be sure that your server can access GitHub ${plain}` | ${red}下载 x-ui 失败，请确认服务器可访问 GitHub ${plain} |
| 249 | `${red}Error: Certificate or private key file not found for domain: $domain.${plain}` | ${red}错误：未找到域名 $domain 的证书或私钥文件。${plain} |
| 250 | `${red}Error: File does not exist! Try again.${plain}` | ${red}错误：文件不存在！请重试。${plain} |
| 251 | `${red}Error: File exists but is not readable (check permissions)!${plain}` | ${red}错误：文件存在但无法读取（请检查权限）！${plain} |
| 252 | `${red}Error: File is empty!${plain}` | ${red}错误：文件为空！${plain} |
| 253 | `${red}Error:${plain} Invalid choice. Please enter 1 or 2.` | ${red}错误：${plain} 选择无效，请输入 1 或 2。 |
| 254 | `${red}Extracted x-ui archive is missing the x-ui binary -- the previous installation has already been removed, so the panel will not start until a valid archive is installed.${plain}` | ${red}解压后的压缩包中缺少 x-ui 主程序 —— 旧版本已被移除，在装回有效压缩包之前面板无法启动。${plain} |
| 255 | `${red}Extracted x-ui archive is missing the x-ui binary -- the previous installation has already been removed, so the panel will not start until this is fixed; try running the installer again${plain}` | ${red}解压后的 x-ui 包中缺少 x-ui 二进制文件 — 旧安装已被移除，修复前面板无法启动；请重新运行安装脚本${plain} |
| 256 | `${red}Fail2ban installation failed.${plain}` | ${red}Fail2ban 安装失败。${plain} |
| 257 | `${red}Fail2ban service is not running!${plain}` | ${red}Fail2ban 服务未运行！${plain} |
| 258 | `${red}Failed to copy x-ui.service${plain}` | ${red}复制 x-ui.service 失败${plain} |
| 259 | `${red}Failed to create temporary credentials file.${plain}` | ${red}创建临时凭据文件失败。${plain} |
| 260 | `${red}Failed to download the checksum for $(basename` | ${red}下载校验和失败：$(basename |
| 261 | `${red}Failed to download the checksum for $(basename "${file}") (HTTP ${code})${plain}` | ${red}下载 $(basename "${file}") 的校验值失败（HTTP ${code}）${plain} |
| 262 | `${red}Failed to download x-ui.rc${plain}` | ${red}下载 x-ui.rc 失败${plain} |
| 263 | `${red}Failed to download x-ui.sh${plain}` | ${red}下载 x-ui.sh 失败${plain} |
| 264 | `${red}Failed to enable BBR. Please check your system configuration.${plain}` | ${red}开启 BBR 失败，请检查系统配置。${plain} |
| 265 | `${red}Failed to extract the x-ui release archive -- the previous installation has already been removed, so the panel will not start until a valid archive is installed.${plain}` | ${red}解压 x-ui 发布包失败 —— 旧版本已被移除，在装回有效压缩包之前面板无法启动。${plain} |
| 266 | `${red}Failed to extract the x-ui release archive -- the previous installation has already been removed, so the panel will not start until this is fixed; try running the installer again${plain}` | ${red}解压 x-ui 发布包失败 — 旧安装已被移除，修复前面板无法启动；请重新运行安装脚本${plain} |
| 267 | `${red}Failed to fetch x-ui version, it may be due to GitHub API restrictions, please try it later${plain}` | ${red}获取 x-ui 版本失败，可能是 GitHub API 限制，请稍后重试${plain} |
| 268 | `${red}Failed to install acme.sh${plain}` | ${red}安装 acme.sh 失败${plain} |
| 269 | `${red}Failed to install x-ui.rc${plain}` | ${red}安装 x-ui.rc 失败${plain} |
| 270 | `${red}Failed to install x-ui.service file${plain}` | ${red}安装 x-ui.service 文件失败${plain} |
| 271 | `${red}Failed to install x-ui.service from GitHub (${script_ref}) -- the release tarball did not ship one either${plain}` | ${red}从 GitHub（${script_ref}）安装 x-ui.service 失败 — 发布包中同样未提供该文件${plain} |
| 272 | `${red}Failed to install x-ui.sh${plain}` | ${red}安装 x-ui.sh 失败${plain} |
| 273 | `${red}Failed to issue IP certificate${plain}` | ${red}申请 IP 证书失败${plain} |
| 274 | `${red}Failed to replace BBR with CUBIC. Please check your system configuration.${plain}` | ${red}将 BBR 替换为 CUBIC 失败，请检查系统配置。${plain} |
| 275 | `${red}Failed to update the menu.${plain}` | ${red}菜单更新失败。${plain} |
| 276 | `${red}Failed to write PostgreSQL credentials to ${PG_CRED_FILE}${plain}` | ${red}无法将 PostgreSQL 凭据写入 ${PG_CRED_FILE}${plain} |
| 277 | `${red}Fatal error: ${plain} Please run this script with root privilege` | ${red}严重错误：${plain} 请以 root 权限运行本脚本 |
| 278 | `${red}IPv4 address is required${plain}` | ${red}需要提供 IPv4 地址${plain} |
| 279 | `${red}Install a release that ships it, or 'dev' for the rolling build. Your existing installation has not been touched.${plain}` | ${red}请安装包含该文件的版本，或使用 'dev' 滚动构建。您现有的安装未被改动。${plain} |
| 280 | `${red}Install a release that ships it, or \'dev\' for the rolling build. Your existing installation has not been touched.${plain}` | ${red}请安装随包附带该文件的版本，或使用 \'dev\' 滚动构建。您现有的安装未被改动。${plain} |
| 281 | `${red}Install aborted.${plain}` | ${red}安装已中止。${plain} |
| 282 | `${red}Installing certificate failed, exiting.${plain}` | ${red}证书安装失败，正在退出。${plain} |
| 283 | `${red}Invalid IP address format! Please try again.${plain}` | ${red}IP 地址格式无效！请重新输入。${plain} |
| 284 | `${red}Invalid IPv4 address: $ipv4${plain}` | ${red}IPv4 地址无效：$ipv4${plain} |
| 285 | `${red}Invalid domain format: ${domain}. Please enter a valid domain name.${plain}` | ${red}域名格式无效：${domain}，请输入有效的域名。${plain} |
| 286 | `${red}Invalid option. Please select a valid number.${plain}` | ${red}无效选项，请输入有效数字。${plain} |
| 287 | `${red}Invalid option. Please select a valid number.${plain}` | ${red}无效选项，请输入正确的数字。${plain} |
| 288 | `${red}Invalid option. Skipping SSL setup.${plain}` | ${red}选项无效，跳过 SSL 配置。${plain} |
| 289 | `${red}Invalid port provided. Falling back to 80.${plain}` | ${red}输入的端口无效，回退到 80。${plain} |
| 290 | `${red}Invalid port provided.${plain}` | ${red}输入的端口无效。${plain} |
| 291 | `${red}Issuing certificate failed, please check logs.${plain}` | ${red}签发证书失败，请查看日志。${plain} |
| 292 | `${red}Nothing is listening on port 5432 - the database is not running.${plain}` | ${red}端口 5432 无监听，数据库未运行。${plain} |
| 293 | `${red}Please use a newer version (at least v2.3.5). Exiting installation.${plain}` | ${red}请使用更新的版本（至少 v2.3.5），退出安装。${plain} |
| 294 | `${red}Port ${WebPort} is busy; cannot proceed in non-interactive mode.${plain}` | ${red}端口 ${WebPort} 已被占用，非交互模式下无法继续。${plain} |
| 295 | `${red}Port ${WebPort} is busy; cannot proceed.${plain}` | ${red}端口 ${WebPort} 已被占用，无法继续。${plain} |
| 296 | `${red}PostgreSQL installation failed in non-interactive mode; aborting.${plain}` | ${red}非交互模式下 PostgreSQL 安装失败，中止。${plain} |
| 297 | `${red}PostgreSQL installation failed.${plain}` | ${red}PostgreSQL 安装失败。${plain} |
| 298 | `${red}SSL certificate setup failed for domain mode.${plain}` | ${red}域名模式的 SSL 证书配置失败。${plain} |
| 299 | `${red}Some ${name} could not be updated. Check the errors above.${plain}` | ${red}部分 ${name} 更新失败，请查看上方错误信息。${plain} |
| 300 | `${red}Unable to read webBasePath; leaving existing settings unchanged.${plain}` | ${red}无法读取 webBasePath，保持现有设置不变。${plain} |
| 301 | `${red}Unsupported CPU architecture!${plain}` | ${red}不支持的 CPU 架构！${plain} |
| 302 | `${red}Unsupported distro for automatic PostgreSQL install: ${release}${plain}` | ${red}当前发行版不支持自动安装 PostgreSQL：${release}${plain} |
| 303 | `${red}Unsupported operating system. Please check the script and install the necessary packages manually.${plain}` | ${red}不支持的操作系统，请检查脚本并手动安装所需软件包。${plain} |
| 304 | `${red}Unsupported operating system. Please uninstall Fail2ban manually.${plain}` | ${red}不支持的操作系统，请手动卸载 Fail2ban。${plain} |
| 305 | `${red}WARNING:${plain} purging removes the PostgreSQL server and ${red}ALL${plain} of its databases on` | ${red}警告：${plain} 清除操作会移除 PostgreSQL 服务及其${red}全部${plain}数据库，影响范围 |
| 306 | `${red}Warning: No Cert and Key found! The panel is not secure.${plain}` | ${red}警告：未找到证书和密钥！面板当前不安全。${plain} |
| 307 | `${red}XUI_SSL_MODE=domain requires a valid XUI_DOMAIN (got: '${XUI_DOMAIN:-}').${plain}` | ${red}XUI_SSL_MODE=domain 需要有效的 XUI_DOMAIN（当前值为：'${XUI_DOMAIN:-}'）。${plain} |
| 308 | `${red}\u26a0 Panel will be installed WITHOUT SSL/TLS.${plain}` | ${red}\u26a0 面板将在未启用 SSL/TLS 的情况下安装。${plain} |
| 309 | `${red}\u26a0 WARNING: No SSL certificate configured!${plain}` | ${red}\u26a0 警告：未配置 SSL 证书！${plain} |
| 310 | `${red}\u2717 IP certificate setup failed. Please check port 80 is open.${plain}` | ${red}\u2717 IP 证书配置失败，请检查 80 端口是否开放。${plain} |
| 311 | `${red}update_geofiles: unknown dataset '${1}'${plain}` | ${red}update_geofiles：未知数据集 '${1}'${plain} |
| 312 | `${red}update_geofiles: unknown dataset \'${1}\'${plain}` | ${red}update_geofiles：未知数据集 \'${1}\'${plain} |
| 313 | `${red}⚠ Panel will be installed WITHOUT SSL/TLS.${plain}` | ${red}⚠ 面板将不启用 SSL/TLS 安装。${plain} |
| 314 | `${red}⚠ WARNING: No SSL certificate configured!${plain}` | ${red}⚠ 警告：尚未配置 SSL 证书！${plain} |
| 315 | `${red}✗ IP certificate setup failed. Please check port 80 is open.${plain}` | ${red}✗ IP 证书申请失败，请检查 80 端口是否放通。${plain} |
| 316 | `${yellow} Back Up downloads a pg_dump .dump file; Restore reloads it via pg_restore.${plain}` | ${yellow} 备份会下载 pg_dump 生成的 .dump 文件；恢复则通过 pg_restore 重新载入。${plain} |
| 317 | `${yellow} \u2022 A reverse proxy (nginx, Caddy, Traefik) terminates TLS for you, or${plain}` | ${yellow} \u2022 由反向代理（nginx、Caddy、Traefik）为您终止 TLS，或${plain} |
| 318 | `${yellow} \u2022 You access the panel exclusively via SSH tunnel${plain}` | ${yellow} \u2022 您仅通过 SSH 隧道访问面板${plain} |
| 319 | `${yellow} • A reverse proxy (nginx, Caddy, Traefik) terminates TLS for you, or${plain}` | ${yellow} • 由反向代理（nginx、Caddy、Traefik）为您终止 TLS，或者${plain} |
| 320 | `${yellow} • You access the panel exclusively via SSH tunnel${plain}` | ${yellow} • 仅通过 SSH 隧道访问面板${plain} |
| 321 | `${yellow}Access URL: http://${server_ip}:${existing_port}${existing_webBasePath}${plain}` | ${yellow}访问地址：http://${server_ip}:${existing_port}${existing_webBasePath}${plain} |
| 322 | `${yellow}Alternative: point a reverse proxy (nginx/Caddy) at 127.0.0.1:${panel_port} and let it terminate TLS.${plain}` | ${yellow}备选方案：将反向代理（nginx/Caddy）指向 127.0.0.1:${panel_port} 并由其终止 TLS。${plain} |
| 323 | `${yellow}Auto renew setup had issues, certificate details:${plain}` | ${yellow}自动续期设置出现问题，证书详情：${plain} |
| 324 | `${yellow}BBR is not currently enabled.${plain}` | ${yellow}当前未开启 BBR。${plain} |
| 325 | `${yellow}Ban log file is empty${plain}` | ${yellow}封禁日志文件为空${plain} |
| 326 | `${yellow}Certificate files are at:${plain}` | ${yellow}证书文件位于：${plain} |
| 327 | `${yellow}Certificate files not found${plain}` | ${yellow}未找到证书文件${plain} |
| 328 | `${yellow}Certificate valid for ~6 days, auto-renews via acme.sh cron job.${plain}` | ${yellow}证书有效期约 6 天，由 acme.sh 定时任务自动续期。${plain} |
| 329 | `${yellow}Choose SSL certificate setup method:${plain}` | ${yellow}请选择 SSL 证书配置方式：${plain} |
| 330 | `${yellow}Could not back up bin/ -- custom files there will not be preserved across this update${plain}` | ${yellow}无法备份 bin/ — 其中的自定义文件在本次更新后不会被保留${plain} |
| 331 | `${yellow}Could not enable the EPEL repository; fail2ban is only available from EPEL on this distro.${plain}` | ${yellow}无法启用 EPEL 源；该发行版中的 fail2ban 仅由 EPEL 提供。${plain} |
| 332 | `${yellow}Default credentials detected. Security update required...${plain}` | ${yellow}检测到默认凭据，需要进行安全更新...${plain} |
| 333 | `${yellow}Default listener is port 80. If you choose another port, ensure external port 80 forwards to it.${plain}` | ${yellow}默认监听端口为 80。若选择其他端口，请确保外部 80 端口转发到该端口。${plain} |
| 334 | `${yellow}Existing certificate found for ${domain}, will reuse it.${plain}` | ${yellow}发现 ${domain} 已有证书，将直接复用。${plain} |
| 335 | `${yellow}Fail2ban is already installed.${plain}` | ${yellow}Fail2ban 已安装。${plain} |
| 336 | `${yellow}Fail2ban setup did not finish; IP Limit stays disabled until you run 'x-ui' and open the IP Limit menu. Continuing.${plain}` | ${yellow}Fail2ban 配置未完成；IP 限制将保持禁用，直到您运行 'x-ui' 并打开 IP 限制菜单。继续执行。${plain} |
| 337 | `${yellow}Fail2ban setup did not finish; IP Limit stays disabled until you run \'x-ui\' and open the IP Limit menu. Continuing.${plain}` | ${yellow}Fail2ban 配置未完成；在您运行 \'x-ui\' 并打开 IP 限制菜单之前，该功能保持禁用。继续执行。${plain} |
| 338 | `${yellow}Failed to install acme.sh, skipping SSL setup${plain}` | ${yellow}安装 acme.sh 失败，跳过 SSL 配置${plain} |
| 339 | `${yellow}Failed to install certificate${plain}` | ${yellow}安装证书失败${plain} |
| 340 | `${yellow}Failed to issue certificate for ${domain}${plain}` | ${yellow}为 ${domain} 申请证书失败${plain} |
| 341 | `${yellow}Found incomplete acme.sh state for ${domain} (no valid certificate files); cleaning it up and re-issuing.${plain}` | ${yellow}发现 ${domain} 的 acme.sh 状态不完整（无有效证书文件），将清理后重新签发。${plain} |
| 342 | `${yellow}Generated random port: ${config_port}${plain}` | ${yellow}已生成随机端口：${config_port}${plain} |
| 343 | `${yellow}If XUI_DB_FOLDER or XUI_LOG_FOLDER points outside /etc/x-ui and /var/log/x-ui, the panel may not be able to write to it under ProtectSystem=full.${plain}` | ${yellow}如果 XUI_DB_FOLDER 或 XUI_LOG_FOLDER 指向 /etc/x-ui 与 /var/log/x-ui 之外，在 ProtectSystem=full 下面板可能无法写入。${plain} |
| 344 | `${yellow}Installing PostgreSQL client tools (pg_dump/pg_restore) for in-panel backup...${plain}` | ${yellow}正在安装 PostgreSQL 客户端工具（pg_dump/pg_restore）以支持面板内备份...${plain} |
| 345 | `${yellow}Installing PostgreSQL client tools (pg_dump/pg_restore)...${plain}` | ${yellow}正在安装 PostgreSQL 客户端工具（pg_dump/pg_restore）...${plain} |
| 346 | `${yellow}Installing PostgreSQL locally (non-interactive)...${plain}` | ${yellow}正在本机安装 PostgreSQL（非交互模式）...${plain} |
| 347 | `${yellow}Installing PostgreSQL — this may take a moment...${plain}` | ${yellow}正在安装 PostgreSQL — 可能需要一些时间...${plain} |
| 348 | `${yellow}Installing the rolling dev build (tag: dev-latest). This is a per-commit pre-release, not a stable version.${plain}` | ${yellow}正在安装滚动开发版（标签：dev-latest）。这是逐提交的预发布版本，不是稳定版。${plain} |
| 349 | `${yellow}It's recommended to put x-ui restart at the end${plain}` | ${yellow}建议将 x-ui restart 放在最后${plain} |
| 350 | `${yellow}Let's Encrypt SSL Certificate for IP Address${plain}` | ${yellow}为 IP 地址申请 Let's Encrypt SSL 证书${plain} |
| 351 | `${yellow}Let's Encrypt now supports both domains and IP addresses!${plain}` | ${yellow}Let's Encrypt 现已支持域名和 IP 地址两种证书！${plain} |
| 352 | `${yellow}Let\'s Encrypt now supports both domains and IP addresses!${plain}` | ${yellow}Let\'s Encrypt 现已支持域名和 IP 地址两种证书！${plain} |
| 353 | `${yellow}Login credentials and cookies will travel as plain HTTP.${plain}` | ${yellow}登录凭据和 Cookie 将以明文 HTTP 传输。${plain} |
| 354 | `${yellow}No SSL certificate is configured; the panel is served over HTTP.${plain}` | ${yellow}未配置 SSL 证书，面板通过 HTTP 提供服务。${plain} |
| 355 | `${yellow}No ban entries found${plain}` | ${yellow}未找到封禁记录${plain} |
| 356 | `${yellow}No checksum published for this release, skipping verification${plain}` | ${yellow}该版本未发布校验和，跳过校验${plain} |
| 357 | `${yellow}No recent system ban activities found${plain}` | ${yellow}未发现最近的系统封禁记录${plain} |
| 358 | `${yellow}Note: IP certificates are valid for ~6 days and will auto-renew.${plain}` | ${yellow}注意：IP 证书有效期约 6 天，会自动续期。${plain} |
| 359 | `${yellow}Note: Port 80 must be open and accessible from the internet${plain}` | ${yellow}注意：80 端口必须开放且可从公网访问${plain} |
| 360 | `${yellow}Note: You are responsible for renewing these files externally.${plain}` | ${yellow}注意：您需要自行在外部续期这些证书文件。${plain} |
| 361 | `${yellow}Note: systemd ${version} ignores part of the hardening in x-ui.service; the panel still starts.${plain}` | ${yellow}注意：systemd ${version} 会忽略 x-ui.service 中的部分加固配置；面板仍可正常启动。${plain} |
| 362 | `${yellow}Only safe when:${plain}` | ${yellow}仅在以下情况才安全：${plain} |
| 363 | `${yellow}Operation canceled.${plain}` | ${yellow}操作已取消。${plain} |
| 364 | `${yellow}Panel will listen on all interfaces over plain HTTP. Make sure something else is terminating TLS in front of it.${plain}` | ${yellow}面板将在所有网卡上以纯 HTTP 监听，请确保前方有其他组件负责终止 TLS。${plain} |
| 365 | `${yellow}Panel will restart to apply SSL certificate...${plain}` | ${yellow}面板将重启以应用 SSL 证书...${plain} |
| 366 | `${yellow}Please ensure port ${WebPort} is reachable (or forwarded from external port 80)${plain}` | ${yellow}请确保端口 ${WebPort} 可访问（或已从外部 80 端口转发）${plain} |
| 367 | `${yellow}Please ensure port 80 is open and try again later with: x-ui${plain}` | ${yellow}请确认 80 端口已开放，稍后运行 x-ui 重试${plain} |
| 368 | `${yellow}Port ${WebPort} is in use.${plain}` | ${yellow}端口 ${WebPort} 已被占用。${plain} |
| 369 | `${yellow}Port 80 must be open and accessible from the internet.${plain}` | ${yellow}80 端口必须开放且可从公网访问。${plain} |
| 370 | `${yellow}PostgreSQL ${PG_TARGET_MAJOR} is not available for this system; installing the distribution's PostgreSQL instead.${plain}` | ${yellow}当前系统不支持 PostgreSQL ${PG_TARGET_MAJOR}，改为安装发行版自带的 PostgreSQL。${plain} |
| 371 | `${yellow}Press enter to return to the main menu: ${plain}` | ${yellow}按回车键返回主菜单：${plain} |
| 372 | `${yellow}Reminder: Let's Encrypt still connects on port 80; forward external port 80 to ${WebPort}.${plain}` | ${yellow}提醒：Let's Encrypt 仍会连接 80 端口，请将外部 80 端口转发到 ${WebPort}。${plain} |
| 373 | `${yellow}Removing conflicts of [3x-ipl] in jail (${file})!${plain}` | ${yellow}正在移除 jail（${file}）中 [3x-ipl] 的冲突配置！${plain} |
| 374 | `${yellow}Resetting Web Base Path${plain}` | ${yellow}正在重置 Web 根路径${plain} |
| 375 | `${yellow}Restarting panel to apply the new web base path...${plain}` | ${yellow}正在重启面板以应用新的 Web 根路径...${plain} |
| 376 | `${yellow}Run 'x-ui' and choose SSL Certificate Management to set one up.${plain}` | ${yellow}运行 'x-ui' 并选择「SSL 证书管理」进行配置。${plain} |
| 377 | `${yellow}Run \'x-ui\' and choose SSL Certificate Management to set one up.${plain}` | ${yellow}运行 \'x-ui\' 并选择「SSL 证书管理」进行配置。${plain} |
| 378 | `${yellow}SSL is strongly recommended. Skip only if a reverse proxy${plain}` | ${yellow}强烈建议启用 SSL。仅在反向代理${plain} |
| 379 | `${yellow}SSL setup may have completed, but domain extraction failed${plain}` | ${yellow}SSL 配置可能已完成，但域名解析失败${plain} |
| 380 | `${yellow}Service files not found in tar.gz, downloading from GitHub...${plain}` | ${yellow}tar.gz 中未找到服务文件，正在从 GitHub 下载...${plain} |
| 381 | `${yellow}Set XUI_DB_DSN to use an existing server, or XUI_DB_TYPE=sqlite.${plain}` | ${yellow}请设置 XUI_DB_DSN 以使用已有服务器，或设置 XUI_DB_TYPE=sqlite。${plain} |
| 382 | `${yellow}Skipping panel path setting.${plain}` | ${yellow}跳过面板证书路径设置。${plain} |
| 383 | `${yellow}Stopping panel temporarily...${plain}` | ${yellow}正在临时停止面板...${plain} |
| 384 | `${yellow}The certificate also covers:${plain}` | ${yellow}该证书同时覆盖：${plain} |
| 385 | `${yellow}This copies your current SQLite data into a PostgreSQL database,${plain}` | ${yellow}此操作会将当前的 SQLite 数据复制到 PostgreSQL 数据库，${plain} |
| 386 | `${yellow}This panel was using PostgreSQL.${plain}` | ${yellow}本面板此前使用的是 PostgreSQL。${plain} |
| 387 | `${yellow}This x-ui.sh predates 'x-ui setup-fail2ban'; skipping Fail2ban auto-setup.${plain}` | ${yellow}此 x-ui.sh 版本早于 'x-ui setup-fail2ban'，跳过 Fail2ban 自动配置。${plain} |
| 388 | `${yellow}This x-ui.sh predates \'x-ui setup-fail2ban\'; skipping Fail2ban auto-setup.${plain}` | ${yellow}此 x-ui.sh 版本早于 \'x-ui setup-fail2ban\'，跳过 Fail2ban 自动配置。${plain} |
| 389 | `${yellow}Unable to get jail status${plain}` | ${yellow}无法获取 jail 状态${plain} |
| 390 | `${yellow}Unknown XUI_SSL_MODE='${XUI_SSL_MODE}', defaulting to none (HTTP).${plain}` | ${yellow}未知的 XUI_SSL_MODE='${XUI_SSL_MODE}'，默认使用 none（HTTP）。${plain} |
| 391 | `${yellow}Updating Menu${plain}` | ${yellow}正在更新菜单${plain} |
| 392 | `${yellow}Use option 2 to migrate your SQLite data and switch the panel to PostgreSQL.${plain}` | ${yellow}使用选项 2 迁移 SQLite 数据并将面板切换到 PostgreSQL。${plain} |
| 393 | `${yellow}Warning: Could not set certificate paths automatically${plain}` | ${yellow}警告：无法自动设置证书路径${plain} |
| 394 | `${yellow}Warning: could not refresh ${xui_service}/x-ui.service.d/10-xui-sandbox.conf.${plain}` | ${yellow}警告：无法刷新 ${xui_service}/x-ui.service.d/10-xui-sandbox.conf。${plain} |
| 395 | `${yellow}Warning: could not update pg_hba.conf; PostgreSQL may reject the panel's TCP login (ident auth).${plain}` | ${yellow}警告：无法更新 pg_hba.conf，PostgreSQL 可能会拒绝面板的 TCP 登录（ident 认证）。${plain} |
| 396 | `${yellow}Warning: failed to write ${result_file}.${plain}` | ${yellow}警告：写入 ${result_file} 失败。${plain} |
| 397 | `${yellow}WebBasePath is missing or set to root. Generating a new one...${plain}` | ${yellow}WebBasePath 缺失或设置为根路径，正在生成新的...${plain} |
| 398 | `${yellow}XUI_ENABLE_FAIL2BAN=${XUI_ENABLE_FAIL2BAN}, skipping Fail2ban auto-setup.${plain}` | ${yellow}XUI_ENABLE_FAIL2BAN=${XUI_ENABLE_FAIL2BAN}，跳过 Fail2ban 自动配置。${plain} |
| 399 | `${yellow}XUI_ENABLE_FAIL2BAN=${XUI_ENABLE_FAIL2BAN}, skipping Fail2ban setup.${plain}` | ${yellow}XUI_ENABLE_FAIL2BAN=${XUI_ENABLE_FAIL2BAN}，跳过 Fail2ban 配置。${plain} |
| 400 | `${yellow}You can get a Let\'s Encrypt certificate for your IP address (valid ~6 days, auto-renews).${plain}` | ${yellow}可以为 IP 地址申请 Let\'s Encrypt 证书（有效期约 6 天，自动续期）。${plain} |
| 401 | `${yellow}You can try again via main menu option 20 (SSL Certificate Management).${plain}` | ${yellow}可通过主菜单 20 项（SSL 证书管理）重试。${plain} |
| 402 | `${yellow}Your Panel Port is: ${config_port}${plain}` | ${yellow}您的面板端口为：${config_port}${plain} |
| 403 | `${yellow}Your input ${WebPort} is invalid, will use default port 80.${plain}` | ${yellow}您输入的 ${WebPort} 无效，将使用默认端口 80。${plain} |
| 404 | `${yellow}\u26a0 Could not install pg_dump/pg_restore. In-panel database backup/restore will be unavailable until you install the postgresql-client package.${plain}` | ${yellow}\u26a0 无法安装 pg_dump/pg_restore。在安装 postgresql-client 包之前，面板内的数据库备份/恢复功能不可用。${plain} |
| 405 | `${yellow}\u26a0 IMPORTANT: Save these credentials securely!${plain}` | ${yellow}\u26a0 重要：请妥善保存这些凭据！${plain} |
| 406 | `${yellow}\u26a0 SSL Certificate: Enabled and configured${plain}` | ${yellow}\u26a0 SSL 证书：已启用并配置完成${plain} |
| 407 | `${yellow}\u26a0 SSL Certificate: Skipped — panel is HTTP-only. Use a reverse proxy or SSH tunnel.${plain}` | ${yellow}\u26a0 SSL 证书：已跳过 — 面板仅支持 HTTP，请使用反向代理或 SSH 隧道。${plain} |
| 408 | `${yellow}\u26a0 Save the password — it is not stored anywhere else in plain text.${plain}` | ${yellow}\u26a0 请保存该密码 — 其他位置不会再以明文存储。${plain} |
| 409 | `${yellow}\u26a0 The panel reads these credentials from ${xui_env_file}.${plain}` | ${yellow}\u26a0 面板从 ${xui_env_file} 读取这些凭据。${plain} |
| 410 | `${yellow}acme.sh will automatically renew and reload x-ui before expiry.${plain}` | ${yellow}acme.sh 会在证书过期前自动续期并重载 x-ui。${plain} |
| 411 | `${yellow}firewalld was pulled in by fail2ban and has been disabled so it does not block your ports after a reboot` | ${yellow}firewalld 是被 fail2ban 一并安装的，现已禁用，避免重启后拦截您的端口 |
| 412 | `${yellow}or SSH tunnel handles TLS for you.${plain}` | ${yellow}或 SSH 隧道已为您处理 TLS 时才跳过。${plain} |
| 413 | `${yellow}then switches the panel to PostgreSQL and restarts it.${plain}` | ${yellow}然后将面板切换到 PostgreSQL 并重启。${plain} |
| 414 | `${yellow}x-ui CLI not found; skipping Fail2ban auto-setup.${plain}` | ${yellow}未找到 x-ui 命令行工具，跳过 Fail2ban 自动配置。${plain} |
| 415 | `${yellow}x-ui settings:${plain}` | ${yellow}x-ui 设置：${plain} |
| 416 | `${yellow}⚠ Could not install pg_dump/pg_restore. In-panel database backup/restore will be unavailable until you install the postgresql-client package.${plain}` | ${yellow}⚠ 未能安装 pg_dump/pg_restore，面板内的数据库备份/恢复不可用，请安装 postgresql-client 包。${plain} |
| 417 | `${yellow}⚠ IMPORTANT: Save these credentials securely!${plain}` | ${yellow}⚠ 重要：请妥善保存以上凭据！${plain} |
| 418 | `${yellow}⚠ SSL Certificate: Enabled and configured${plain}` | ${yellow}⚠ SSL 证书：已启用并完成配置${plain} |
| 419 | `${yellow}⚠ SSL Certificate: Skipped — panel is HTTP-only. Use a reverse proxy or SSH tunnel.${plain}` | ${yellow}⚠ SSL 证书：已跳过 —— 面板仅支持 HTTP，请使用反向代理或 SSH 隧道。${plain} |
| 420 | `${yellow}⚠ Save the password — it is not stored anywhere else in plain text.${plain}` | ${yellow}⚠ 请保存密码 —— 除此之外没有任何地方以明文存放它。${plain} |
| 421 | `${yellow}⚠ The panel reads these credentials from ${xui_env_file}.${plain}` | ${yellow}⚠ 面板从 ${xui_env_file} 读取这些凭据。${plain} |
| 422 | `'` | \\' |
| 423 | `) BAN [Email] = <F-USER> [IP] = <ip> banned for <bantime> seconds.` | ) 封禁 [Email] = <F-USER> [IP] = <ip> 被封禁 <bantime> 秒。 |
| 424 | `): expected ${expected:-<none>}, got ${actual}${plain}` | )：期望 ${expected:-<none>}，实际 ${actual}${plain} |
| 425 | `): expected ${expected_sha256:-<none>}, got ${actual_sha256}` | )：期望 ${expected_sha256:-<none>}，实际 ${actual_sha256} |
| 426 | `****** Instructions for Use ******` | ****** 使用说明 ****** |
| 427 | `1) Install PostgreSQL locally and create a dedicated user/db (recommended)` | 1) 本地安装 PostgreSQL 并创建专用用户与数据库（推荐） |
| 428 | `1) Retry local install` | 1) 重试本地安装 |
| 429 | `1) Rule numbers` | 1) 按规则编号 |
| 430 | `1) SQLite (default — recommended for < 500 clients)` | 1) SQLite （默认，客户端少于 500 时推荐） |
| 431 | `1. A Cloudflare API Token (recommended, scoped to Zone:DNS:Edit) or the Global API Key + registered email.` | 1. Cloudflare API Token（推荐，权限范围 Zone:DNS:Edit）或全局 API Key + 注册邮箱。 |
| 432 | `1. Use default IP (127.0.0.1)` | 1. 使用默认 IP (127.0.0.1) |
| 433 | `2) Enter an external DSN instead` | 2) 改为输入外部 DSN |
| 434 | `2) Ports` | 2) 按端口 |
| 435 | `2) PostgreSQL (recommended for high client counts / many nodes)` | 2) PostgreSQL （客户端数量大 / 多节点时推荐） |
| 436 | `2) Use an existing PostgreSQL server (enter DSN)` | 2) 使用已有的 PostgreSQL 服务器（输入 DSN） |
| 437 | `2. Set a custom IP` | 2. 设置自定义 IP |
| 438 | `2. The Domain Name.` | 2. 域名。 |
| 439 | `3) Abort install` | 3) 中止安装 |
| 440 | `3. Once the certificate is issued, you will be prompted to set the certificate for the panel (optional).` | 3. 证书签发后，会提示您为面板设置该证书（可选）。 |
| 441 | `3X-UI Panel Management Script` | 3X-UI 面板管理脚本 |
| 442 | `4) Fall back to SQLite` | 4) 改用 SQLite |
| 443 | `4. The script also supports automatic renewal of the SSL certificate after installation.` | 4. 该脚本还支持安装后自动续期 SSL 证书。 |
| 444 | `A PostgreSQL database was created in this session:` | 本次会话已创建 PostgreSQL 数据库： |
| 445 | `Activating firewall...` | 正在启用防火墙... |
| 446 | `All Logs cleared.` | 所有日志已清空。 |
| 447 | `All panel settings have been reset to default.` | 所有面板设置已恢复为默认值。 |
| 448 | `Also purge PostgreSQL and delete all of its data?` | 是否同时清除 PostgreSQL 并删除其全部数据？ |
| 449 | `Arch: $(arch)` | 架构：$(arch) |
| 450 | `Are you sure to reset the username and password of the panel?` | 确定要重置面板的用户名和密码吗？ |
| 451 | `Are you sure you want to reset all panel settings, Account data will not be lost, Username and password will not change` | 确定要重置所有面板设置吗？账号数据不会丢失，用户名和密码也不会改变 |
| 452 | `Are you sure you want to reset the web base path? (y/n):` | 确定要重置 Web 根路径吗？(y/n)： |
| 453 | `Are you sure you want to uninstall the panel? xray will also uninstalled!` | 确定要卸载面板吗？xray 也会被一并卸载！ |
| 454 | `Are you using a Cloudflare API Token or Global API Key? (t/g) [Default t]:` | 您使用的是 Cloudflare API Token 还是全局 API Key？(t/g) [默认 t]： |
| 455 | `Auto renew failed, certificate details:` | 自动续期设置失败，证书详情： |
| 456 | `Auto renew succeeded, certificate details:` | 自动续期设置成功，证书详情： |
| 457 | `Auto update setup failed, script exiting...` | 自动更新设置失败，脚本退出... |
| 458 | `Autostart is controlled by the Docker restart policy (e.g. 'restart: unless-stopped' in docker-compose.yml).` | 开机自启由 Docker 重启策略控制（例如 docker-compose.yml 中的 'restart: unless-stopped'）。 |
| 459 | `Available domains:` | 可用域名： |
| 460 | `Beginning to install x-ui ${tag_version}` | 开始安装 x-ui ${tag_version} |
| 461 | `Bind the panel to 127.0.0.1 only? (recommended — forces SSH tunnel / reverse-proxy access) [y/N]:` | 是否只将面板绑定到 127.0.0.1？（推荐 — 强制通过 SSH 隧道 / 反向代理访问）[y/N]： |
| 462 | `Cancelled` | 已取消 |
| 463 | `Certificate file path (fullchain):` | 证书文件路径（fullchain）： |
| 464 | `Certificate files installed successfully` | 证书文件安装成功 |
| 465 | `Certificate files not found after installation` | 安装后未找到证书文件 |
| 466 | `Certificate forcefully renewed for domain: $domain` | 域名 $domain 的证书已强制续期 |
| 467 | `Certificate installation failed, script exiting...` | 证书安装失败，脚本退出... |
| 468 | `Certificate installed successfully, Turning on automatic updates...` | 证书安装成功，正在开启自动更新... |
| 469 | `Certificate issuance failed, script exiting...` | 证书签发失败，脚本退出... |
| 470 | `Certificate issued successfully for IP: ${server_ip}` | 已成功为 IP ${server_ip} 签发证书 |
| 471 | `Certificate issued successfully, Installing...` | 证书签发成功，正在安装... |
| 472 | `Certificate or private key file not found.` | 未找到证书或私钥文件。 |
| 473 | `Certificate or private key not found for domain: $domain.` | 域名 $domain 的证书或私钥未找到。 |
| 474 | `Certificate revoked and removed for domain: ${domain}` | 域名 ${domain} 的证书已吊销并删除 |
| 475 | `Change Port` | 修改面板端口 |
| 476 | `Check Status` | 查看运行状态 |
| 477 | `Choose [1]:` | 请选择 [1]： |
| 478 | `Choose an option (default 2 for IP):` | 请选择一个选项（IP 证书默认 2）： |
| 479 | `Choose an option:` | 请选择一个选项： |
| 480 | `Cleared panel certificate paths referencing ${domain}; restarting panel.` | 已清除面板中引用 ${domain} 的证书路径，正在重启面板。 |
| 481 | `Cloudflare SSL Certificate` | Cloudflare SSL 证书 |
| 482 | `Continue?` | 是否继续？ |
| 483 | `Convert between a SQLite ${green}.db${plain} and a portable ${green}.dump${plain} (direction auto-detected).` | 在 SQLite ${green}.db${plain} 与可移植的 ${green}.dump${plain} 之间转换（自动识别方向）。 |
| 484 | `Could not auto-detect server IP from any provider.` | 无法从任何服务商自动检测服务器 IP。 |
| 485 | `Could not determine the Enterprise Linux release; install the PostgreSQL ${want} client tools manually.` | 无法确定 Enterprise Linux 版本，请手动安装 PostgreSQL ${want} 客户端工具。 |
| 486 | `Could not find the running panel process to signal.` | 未找到正在运行的面板进程，无法发送信号。 |
| 487 | `Could not install pg_dump/pg_restore (in-panel DB backup/restore may be unavailable).` | 无法安装 pg_dump/pg_restore（面板内的数据库备份/恢复功能可能不可用）。 |
| 488 | `Could not install pg_dump/pg_restore (panel DB backup may be unavailable).` | 无法安装 pg_dump/pg_restore（面板数据库备份功能可能不可用）。 |
| 489 | `Current UFW rules:` | 当前 UFW 规则： |
| 490 | `Default --reloadcmd for ACME is: ${yellow}x-ui restart` | ACME 默认 --reloadcmd 为：${yellow}x-ui restart |
| 491 | `Default CA, Let'sEncrypt fail, script exiting...` | 默认 CA（Let's Encrypt）失败，脚本退出... |
| 492 | `Deleted the specified ports:` | 已删除指定端口： |
| 493 | `Dev update is complete, Panel has automatically restarted` | 开发版更新完成，面板已自动重启 |
| 494 | `Disable Autostart` | 关闭开机自启 |
| 495 | `Disable autostart on boot` | 关闭开机自启 |
| 496 | `Do you confirm the information and wish to proceed? [y/n]` | 确认以上信息并继续？[y/n] |
| 497 | `Do you have an IPv6 address to include? (leave empty to skip):` | 是否需要包含 IPv6 地址？（留空则跳过）： |
| 498 | `Do you want to delete rules by:` | 请选择删除规则的方式： |
| 499 | `Do you want to disable currently configured two-factor authentication? (y/n):` | 是否取消当前已配置的双重认证？(y/n)： |
| 500 | `Do you want to proceed?` | 是否继续？ |
| 501 | `Domain name cannot be empty. Please try again.` | 域名不能为空，请重新输入。 |
| 502 | `Domain: ${domain} - Certificate or Key missing.` | 域名：${domain} - 缺少证书或私钥。 |
| 503 | `Done. Created ${output}.` | 完成，已创建 ${output}。 |
| 504 | `Done. Wrote ${output}.` | 完成，已写入 ${output}。 |
| 505 | `Downloading and installing panel version $tag_version...` | 正在下载并安装面板版本 $tag_version... |
| 506 | `Dump failed.` | 导出失败。 |
| 507 | `Dumping SQLite database to SQL text:` | 正在将 SQLite 数据库导出为 SQL 文本： |
| 508 | `ERROR: ${dir} is not writable for this process (read-only mount, attribute or full filesystem). The panel's fallback updater cannot run inside the hardened systemd sandbox; update from the panel UI (which uses systemd-run) or run 'x-ui update' in a shell.` | 错误：当前进程无法写入 ${dir}（只读挂载、文件属性或磁盘已满）。面板的备用更新器无法在加固的 systemd 沙箱内运行；请从面板界面更新（使用 systemd-run）或在 shell 中运行 'x-ui update'。 |
| 509 | `ERROR: ${name} is not available for ${ref} (HTTP ${status}). Update to a release that ships it, or to 'dev-latest'. The current installation is untouched.` | 错误：${name} 在 ${ref} 中不可用（HTTP ${status}）。请更新到包含该文件的版本，或使用 'dev-latest'。当前安装未被改动。 |
| 510 | `ERROR: Checksum mismatch for $(basename` | 错误：校验和不匹配：$(basename |
| 511 | `ERROR: Command 'curl' not found.` | 错误：未找到 curl 命令。 |
| 512 | `ERROR: Current x-ui version: unknown` | 错误：当前 x-ui 版本：未知 |
| 513 | `ERROR: Downloaded startup unit x-ui.rc is empty, please be sure that your server can access GitHub` | 错误：下载的启动单元 x-ui.rc 为空，请确认服务器可访问 GitHub |
| 514 | `ERROR: Downloaded x-ui release archive is empty, please be sure that your server can access GitHub` | 错误：下载的 x-ui 发布包为空，请确认服务器可访问 GitHub |
| 515 | `ERROR: Extracted x-ui archive is missing the x-ui binary -- the previous installation has already been removed, so the panel will not start until this is fixed; try running the update again` | 错误：解压后的 x-ui 包中缺少 x-ui 二进制文件 — 旧安装已被移除，修复前面板无法启动；请重新运行更新 |
| 516 | `ERROR: Failed to download startup unit x-ui.rc, please be sure that your server can access GitHub` | 错误：下载启动单元 x-ui.rc 失败，请确认服务器可访问 GitHub |
| 517 | `ERROR: Failed to download the checksum for x-ui-linux-$(arch).tar.gz (HTTP ${sidecar_code})` | 错误：下载 x-ui-linux-$(arch).tar.gz 的校验和失败（HTTP ${sidecar_code}） |
| 518 | `ERROR: Failed to download x-ui, please be sure that your server can access GitHub` | 错误：下载 x-ui 失败，请确认服务器可访问 GitHub |
| 519 | `ERROR: Failed to extract the x-ui release archive -- the previous installation has already been removed, so the panel will not start until this is fixed; try running the update again` | 错误：解压 x-ui 发布包失败 — 旧安装已被移除，修复前面板无法启动；请重新运行更新 |
| 520 | `ERROR: Failed to fetch x-ui version, it may be due to GitHub API restrictions, please try it later` | 错误：获取 x-ui 版本失败，可能是 GitHub API 限制，请稍后重试 |
| 521 | `ERROR: Failed to install startup unit x-ui.rc` | 错误：安装启动单元 x-ui.rc 失败 |
| 522 | `ERROR: Failed to install x-ui.sh script` | 错误：安装 x-ui.sh 脚本失败 |
| 523 | `ERROR: You must be root to run this script!` | 错误：必须以 root 身份运行本脚本！ |
| 524 | `ERROR: x-ui not installed.` | 错误：x-ui 未安装。 |
| 525 | `ERROR: x-ui service unit not installed.` | 错误：未安装 x-ui 服务单元。 |
| 526 | `ERROR: x-ui systemd unit not installed.` | 错误：未安装 x-ui systemd unit。 |
| 527 | `Enable Autostart` | 开启开机自启 |
| 528 | `Enable BBR` | 开启 BBR 加速 |
| 529 | `Enable autostart on boot` | 开启开机自启 |
| 530 | `Enter PostgreSQL DSN (postgres://user:pass@host:port/dbname?sslmode=disable):` | 请输入 PostgreSQL DSN（postgres://user:pass@host:port/dbname?sslmode=disable）： |
| 531 | `Enter another port for acme.sh standalone listener (leave empty to abort):` | 请输入 acme.sh 独立监听使用的其他端口（留空则中止）： |
| 532 | `Enter custom IP to listen on:` | 请输入要监听的 IP： |
| 533 | `Enter port number[1-65535]:` | 请输入端口号 [1-65535]： |
| 534 | `Enter the IP address you want to ban:` | 请输入要封禁的 IP 地址： |
| 535 | `Enter the IP address you want to unban:` | 请输入要解封的 IP 地址： |
| 536 | `Enter the panel version (like 2.4.0):` | 请输入面板版本（例如 2.4.0）： |
| 537 | `Enter the ports you want to delete (e.g. 80,443,2053 or range 400-500):` | 请输入要删除的端口（例如 80,443,2053 或范围 400-500）： |
| 538 | `Enter the ports you want to open (e.g. 80,443,2053 or range 400-500):` | 请输入要开放的端口（例如 80,443,2053 或范围 400-500）： |
| 539 | `Enter the rule numbers you want to delete (1, 2, etc.):` | 请输入要删除的规则编号（如 1, 2 等）： |
| 540 | `Enter your choice (1 or 2):` | 请输入您的选择（1 或 2）： |
| 541 | `Error: Certificate or private key file not found for IP: $server_ip.` | 错误：未找到 IP $server_ip 的证书或私钥文件。 |
| 542 | `Error: Certificate or private key file not found for domain: $CF_Domain.` | 错误：未找到域名 $CF_Domain 的证书或私钥文件。 |
| 543 | `Error: Certificate or private key file not found for domain: $domain.` | 错误：未找到域名 $domain 的证书或私钥文件。 |
| 544 | `Error: Invalid input. Please enter a comma-separated list of ports or a range of ports (e.g. 80,443,2053 or 400-500).` | 错误：输入无效。请输入以逗号分隔的端口列表或端口范围（例如 80,443,2053 或 400-500）。 |
| 545 | `Error: Invalid input. Please enter a comma-separated list of rule numbers.` | 错误：输入无效。请输入以逗号分隔的规则编号。 |
| 546 | `Error: Package manager not found. You may need to install Speedtest manually.` | 错误：未找到包管理器，您可能需要手动安装 Speedtest。 |
| 547 | `Existing certificate found for ${domain}, will reuse it.` | 发现 ${domain} 已有证书，将直接复用。 |
| 548 | `Existing domains and their paths:` | 已有域名及其证书路径： |
| 549 | `Existing domains:` | 已有域名： |
| 550 | `Exit Script` | 退出脚本 |
| 551 | `Extracted x-ui archive is missing the x-ui binary -- the previous installation has already been removed, so the panel will not start until this is fixed; try running the installer again` | 解压后的压缩包缺少 x-ui 主程序 —— 旧版本已被移除，问题修复前面板无法启动；请重新运行安装程序 |
| 552 | `FATAL ERROR: Please run this script with root privilege.` | 严重错误：请以 root 权限运行本脚本。 |
| 553 | `Failed to check the system OS, please contact the author!` | 检测系统 OS 失败，请联系作者！ |
| 554 | `Failed to create directory: ${certPath}` | 创建目录失败：${certPath} |
| 555 | `Failed to delete rule number $rule_number` | 删除规则编号 $rule_number 失败 |
| 556 | `Failed to download script, Please check whether the machine can connect Github` | 下载脚本失败，请检查本机能否连接 GitHub |
| 557 | `Failed to download x-ui` | 下载 x-ui 失败 |
| 558 | `Failed to enable PostgreSQL autostart.` | 开启 PostgreSQL 开机自启失败。 |
| 559 | `Failed to extract the x-ui release archive -- the previous installation has already been removed, so the panel will not start until this is fixed; try running the installer again` | 解压 x-ui 发布包失败 —— 旧版本已被移除，问题修复前面板无法启动；请重新运行安装程序 |
| 560 | `Failed to fetch x-ui version` | 获取 x-ui 版本失败 |
| 561 | `Failed to install acme.sh` | 安装 acme.sh 失败 |
| 562 | `Failed to issue certificate for IP: ${server_ip}` | 为 IP ${server_ip} 签发证书失败 |
| 563 | `Failed to update the menu.` | 更新菜单失败。 |
| 564 | `Firewall Management` | 防火墙管理 |
| 565 | `Firewall is already active` | 防火墙已处于启用状态 |
| 566 | `Follow the steps below to complete the process:` | 请按以下步骤完成操作： |
| 567 | `For security, please configure SSL certificate using main menu option 20 (SSL Certificate Management)` | 为了安全，请通过主菜单 20 项（SSL 证书管理）配置 SSL 证书 |
| 568 | `Found incomplete acme.sh state for ${domain} (no valid certificate files); cleaning it up and re-issuing.` | 发现 ${domain} 的 acme.sh 状态不完整（无有效证书文件），将清理后重新签发。 |
| 569 | `Generate SSL certificate for IP now? [y/N]:` | 现在为 IP 生成 SSL 证书？[y/N]： |
| 570 | `Generated new random login credentials:` | 已生成新的随机登录凭据： |
| 571 | `Got x-ui latest version: ${tag_version}, beginning the installation...` | 已获取 x-ui 最新版本：${tag_version}，开始安装... |
| 572 | `IP Limit Management` | IP 限制管理 |
| 573 | `IP certificate setup failed.` | IP 证书配置失败。 |
| 574 | `If you need to install this panel again, you can use below command:` | 如需重新安装本面板，可使用以下命令： |
| 575 | `In Docker the panel is the container's main process. Restart the container to bring it back up:` | 在 Docker 中面板即容器的主进程，请重启容器以恢复运行： |
| 576 | `In Docker the panel runs as the container's main process.` | 在 Docker 中面板以容器主进程的方式运行。 |
| 577 | `Including IPv6 address: ${ipv6_addr}` | 包含 IPv6 地址：${ipv6_addr} |
| 578 | `Input certificate path (keywords: .crt / fullchain):` | 请输入证书路径（关键字：.crt / fullchain）： |
| 579 | `Input file [${default_db}]:` | 输入文件 [${default_db}]： |
| 580 | `Input file not found: ${input}` | 输入文件未找到：${input} |
| 581 | `Input private key path (keywords: .key / privatekey):` | 请输入私钥路径（关键字：.key / privatekey）： |
| 582 | `Input your domain here:` | 在此输入您的域名： |
| 583 | `Input your email here:` | 在此输入您的邮箱： |
| 584 | `Input your key here:` | 在此输入您的 Key： |
| 585 | `Input your own command` | 手动输入自定义命令 |
| 586 | `Input your token here:` | 在此输入您的 Token： |
| 587 | `Install` | 安装面板 |
| 588 | `Install a specific legacy version` | 安装指定的历史版本 |
| 589 | `Install acme failed, please check logs.` | 安装 acme 失败，请查看日志。 |
| 590 | `Install the panel` | 安装面板 |
| 591 | `Installation of acme.sh failed.` | acme.sh 安装失败。 |
| 592 | `Installation of acme.sh succeeded.` | acme.sh 安装成功。 |
| 593 | `Installed PostgreSQL client tools are version ${have}; version ${want} or newer is required.` | 已安装的 PostgreSQL 客户端工具版本为 ${have}，需要 ${want} 或更高版本。 |
| 594 | `Installing PostgreSQL locally (this may take a moment)...` | 正在本机安装 PostgreSQL（可能需要一些时间）... |
| 595 | `Installing PostgreSQL server and creating a dedicated user/database...` | 正在安装 PostgreSQL 服务并创建专用用户/数据库... |
| 596 | `Installing Speedtest using $pkg_manager...` | 正在使用 $pkg_manager 安装 Speedtest... |
| 597 | `Installing Speedtest using snap...` | 正在使用 snap 安装 Speedtest... |
| 598 | `Installing acme.sh...` | 正在安装 acme.sh... |
| 599 | `Installing certificate failed, exiting.` | 证书安装失败，正在退出。 |
| 600 | `Installing certificate succeeded, enabling auto renew...` | 证书安装成功，正在启用自动续期... |
| 601 | `Installing full chain to:` | 正在安装完整证书链到： |
| 602 | `Installing key to:` | 正在安装私钥到： |
| 603 | `Invalid IPv4 address. Please try again.` | IPv4 地址无效，请重试。 |
| 604 | `Invalid PostgreSQL major version '${want}' (expected a number like 17).` | PostgreSQL 主版本号无效 '${want}'（应为类似 17 的数字）。 |
| 605 | `Invalid domain entered.` | 输入的域名无效。 |
| 606 | `Invalid domain format: ${domain}. Please enter a valid domain name.` | 域名格式无效：${domain}，请输入有效的域名。 |
| 607 | `Invalid port provided.` | 输入的端口无效。 |
| 608 | `Invalid port provided. Falling back to 80.` | 输入的端口无效，将回退到 80。 |
| 609 | `Is ${server_ip} the correct incoming public IPv4 address for this server?` | ${server_ip} 是本服务器的公网入口 IPv4 地址吗？ |
| 610 | `Is ${server_ip} the correct incoming public IPv4 address for this server? [Default y]:` | ${server_ip} 是本服务器的公网入口 IPv4 地址吗？[默认 y]： |
| 611 | `Issuing certificate failed, please check logs.` | 签发证书失败，请查看日志。 |
| 612 | `Issuing certificate for server IP: ${server_ip}` | 正在为服务器 IP 申请证书：${server_ip} |
| 613 | `Issuing certificate succeeded, installing certificates...` | 证书签发成功，正在安装证书... |
| 614 | `It's recommended to put x-ui restart at the end, so it won't raise an error if other services fails` | 建议将 x-ui restart 放在最后，这样其他服务失败时不会中断后续步骤 |
| 615 | `Keep default reloadcmd` | 保持默认 reloadcmd |
| 616 | `LOGI "acme.sh not found, installing..."` | LOGI "未找到 acme.sh，正在安装..." |
| 617 | `Left PostgreSQL installed; its data was not removed.` | 已保留 PostgreSQL 安装，其数据未被删除。 |
| 618 | `Legacy Version` | 安装历史版本 |
| 619 | `Logs Management` | 日志管理 |
| 620 | `Loyalsoldier datasets` | Loyalsoldier 数据集 |
| 621 | `Make sure port ${WebPort} is open and the server is accessible from the internet` | 请确认端口 ${WebPort} 已开放且服务器可从公网访问 |
| 622 | `Manage PostgreSQL client` | 管理 PostgreSQL 客户端 |
| 623 | `Manage logs` | 管理日志 |
| 624 | `Migrate into this database?` | 是否迁移到该数据库？ |
| 625 | `Migrate the database` | 迁移数据库 |
| 626 | `Migrating data into PostgreSQL...` | 正在将数据迁移到 PostgreSQL... |
| 627 | `Migration complete. The panel is now running on PostgreSQL.` | 迁移完成，面板现已运行在 PostgreSQL 上。 |
| 628 | `Migration failed. The panel was NOT switched to PostgreSQL.` | 迁移失败，面板未切换到 PostgreSQL。 |
| 629 | `No PostgreSQL log found.` | 未找到 PostgreSQL 日志。 |
| 630 | `No certificates found to renew.` | 未找到可续期的证书。 |
| 631 | `No certificates found to revoke.` | 未找到可吊销的证书。 |
| 632 | `No certificates found under /root/cert.` | /root/cert 下未找到证书。 |
| 633 | `No certificates found.` | 未找到证书。 |
| 634 | `Not applied, needs a newer systemd: ${missing}.` | 未应用，需要更新版本的 systemd：${missing}。 |
| 635 | `Note: packages installed inside the container are lost when the container is recreated.` | 注意：容器内安装的软件包在容器重建后会丢失。 |
| 636 | `Opened the specified ports:` | 已开放指定端口： |
| 637 | `Output ${output} already exists and will be overwritten. Continue?` | 输出文件 ${output} 已存在，将被覆盖。是否继续？ |
| 638 | `Output file (leave empty to auto-name next to input):` | 输出文件（留空则自动命名在输入文件旁边）： |
| 639 | `Panel certificate (custom path): ${panel_cert}` | 面板证书（自定义路径）：${panel_cert} |
| 640 | `Panel certificate paths set:` | 面板证书路径已设置： |
| 641 | `Panel did not come up. Check logs (main menu option 17). Your SQLite data is left intact.` | 面板未能启动，请查看日志（主菜单选项 17）。您的 SQLite 数据保持完整。 |
| 642 | `Panel installed, Please do not reinstall` | 面板已安装，请勿重复安装 |
| 643 | `Panel is running, No need to start again, If you need to restart, please select restart` | 面板正在运行，无需重复启动；如需重启请选择「重启」 |
| 644 | `Panel login password has been reset to: ${green} ${config_password} ${plain}` | 面板登录密码已重置为：${green} ${config_password} ${plain} |
| 645 | `Panel login username has been reset to: ${green} ${config_account} ${plain}` | 面板登录用户名已重置为：${green} ${config_account} ${plain} |
| 646 | `Panel paths set for IP: $server_ip` | 已为 IP $server_ip 设置面板证书路径 |
| 647 | `Panel paths set for domain: $CF_Domain` | 已为域名 $CF_Domain 设置面板证书路径 |
| 648 | `Panel paths set for domain: $domain` | 已为域名 $domain 设置面板证书路径 |
| 649 | `Panel process is not running inside this container.` | 面板进程未在该容器内运行。 |
| 650 | `Panel restart failed, Please check the log information later` | 面板重启失败，请稍后查看日志 |
| 651 | `Panel restart failed, Probably because it takes longer than two seconds to start, Please check the log information later` | 面板重启失败，可能启动耗时超过两秒，请稍后查看日志 |
| 652 | `Panel state: ${green}Running${plain}` | 面板状态：${green}运行中${plain} |
| 653 | `Panel state: ${red}Not Installed${plain}` | 面板状态：${red}未安装${plain} |
| 654 | `Panel state: ${yellow}Not Running${plain}` | 面板状态：${yellow}未运行${plain} |
| 655 | `Panel stop failed, Probably because the stop time exceeds two seconds, Please check the log information later` | 面板停止失败，可能停止耗时超过两秒，请稍后查看日志 |
| 656 | `Panel stopped, No need to stop again!` | 面板已停止，无需重复停止！ |
| 657 | `Panel version cannot be empty. Exiting.` | 面板版本不能为空，正在退出。 |
| 658 | `Panel will restart to apply SSL certificate...` | 面板将重启以应用 SSL 证书... |
| 659 | `Please choose a domain to set the panel paths:` | 请选择要为其设置面板证书路径的域名： |
| 660 | `Please choose which port to use (default is 80):` | 请选择使用的端口（默认 80）： |
| 661 | `Please enter a domain from the list to renew the SSL certificate:` | 请从列表中选择要续期 SSL 证书的域名： |
| 662 | `Please enter a domain from the list to revoke and remove the certificate:` | 请从列表中选择要吊销并删除证书的域名： |
| 663 | `Please enter domain name certificate issued for:` | 请输入证书对应的域名： |
| 664 | `Please enter new Ban Duration in Minutes [default 30]:` | 请输入新的封禁时长（分钟）[默认 30]： |
| 665 | `Please enter the correct number [0-28]` | 请输入正确的数字 [0-28] |
| 666 | `Please enter your custom reloadcmd:` | 请输入自定义 reloadcmd： |
| 667 | `Please enter your domain name:` | 请输入您的域名： |
| 668 | `Please enter your reloadcmd (example: systemctl reload nginx ; x-ui restart):` | 请输入您的 reloadcmd（示例：systemctl reload nginx ; x-ui restart）： |
| 669 | `Please enter your selection [0-28]:` | 请输入您的选择 [0-28]： |
| 670 | `Please enter your server's public IPv4 address:` | 请输入服务器的公网 IPv4 地址： |
| 671 | `Please install the panel first` | 请先安装面板 |
| 672 | `Please obtain a certificate or set up SSH port forwarding.` | 请申请证书或配置 SSH 端口转发。 |
| 673 | `Please set a domain name:` | 请设置域名： |
| 674 | `Please set the API Token:` | 请设置 API Token： |
| 675 | `Please set the Global API Key:` | 请设置全局 API Key： |
| 676 | `Please set the login password [default is a random password]:` | 请设置登录密码 [默认为随机密码]： |
| 677 | `Please set the login username [default is a random username]:` | 请设置登录用户名 [默认为随机用户名]： |
| 678 | `Please set up the panel port:` | 请设置面板端口： |
| 679 | `Please set up the registered email:` | 请设置注册邮箱： |
| 680 | `Port ${WebPort} is busy; cannot proceed with issuance.` | 端口 ${WebPort} 已被占用，无法继续签发证书。 |
| 681 | `Port ${WebPort} is currently in use.` | 端口 ${WebPort} 当前已被占用。 |
| 682 | `Port ${WebPort} is free and ready for standalone validation.` | 端口 ${WebPort} 空闲，可用于独立验证。 |
| 683 | `Port to use for ACME HTTP-01 listener (default 80):` | ACME HTTP-01 监听端口（默认 80）： |
| 684 | `PostgreSQL (${PG_USER}@${PG_HOST}:${PG_PORT}/${PG_DB})` | PostgreSQL（${PG_USER}@${PG_HOST}:${PG_PORT}/${PG_DB}） |
| 685 | `PostgreSQL (external)` | PostgreSQL（外部） |
| 686 | `PostgreSQL Management` | PostgreSQL 管理 |
| 687 | `PostgreSQL already appears to be installed on this system.` | 当前系统似乎已安装 PostgreSQL。 |
| 688 | `PostgreSQL client tools are already installed (version ${have}).` | 已安装 PostgreSQL 客户端工具（版本 ${have}）。 |
| 689 | `PostgreSQL client tools are ready (version ${have}).` | PostgreSQL 客户端工具已就绪（版本 ${have}）。 |
| 690 | `PostgreSQL client tools are version ${have} after installation but ${want} or newer is required; install them manually.` | 安装后 PostgreSQL 客户端工具版本为 ${have}，但仍需要 ${want} 或更高版本，请手动安装。 |
| 691 | `PostgreSQL does not appear to be installed on this system.` | 当前系统似乎未安装 PostgreSQL。 |
| 692 | `PostgreSQL has been purged.` | PostgreSQL 已清除。 |
| 693 | `PostgreSQL installation failed.` | PostgreSQL 安装失败。 |
| 694 | `PostgreSQL installation failed. Aborting migration.` | PostgreSQL 安装失败，中止迁移。 |
| 695 | `PostgreSQL is installed and ready.` | PostgreSQL 已安装并可用。 |
| 696 | `PostgreSQL is not installed. Use option 1 (Install PostgreSQL) in this menu first.` | 未安装 PostgreSQL，请先使用本菜单的选项 1（安装 PostgreSQL）。 |
| 697 | `PostgreSQL set to start automatically on boot.` | PostgreSQL 已设置为开机自启。 |
| 698 | `PostgreSQL stop signal sent.` | 已发送 PostgreSQL 停止信号。 |
| 699 | `Preset: systemctl reload nginx ; x-ui restart` | 预设：systemctl reload nginx ; systemctl restart x-ui |
| 700 | `Private key file path:` | 私钥文件路径： |
| 701 | `Proceed with Unbanning everyone from IP Limit jail?` | 确认将所有 IP 从 IP 限制名单中解封？ |
| 702 | `Proceed with installation of Fail2ban & IP Limit?` | 确认安装 Fail2ban 与 IP 限制？ |
| 703 | `Rebuilding SQLite database from SQL text:` | 正在根据 SQL 文本重建 SQLite 数据库： |
| 704 | `Refusing to restore into the live database (${default_db}) while x-ui is running.` | x-ui 运行期间，拒绝恢复到正在使用的数据库（${default_db}）。 |
| 705 | `Registered acme.sh auto-renewal hook for ${domain}.` | 已为 ${domain} 注册 acme.sh 自动续期钩子。 |
| 706 | `Reload error` | 重载出错 |
| 707 | `Reloadcmd is: systemctl reload nginx ; x-ui restart` | reloadcmd 为：systemctl reload nginx ; x-ui restart |
| 708 | `Reminder: Let's Encrypt still reaches port 80; forward external port 80 to ${WebPort} for validation.` | 提醒：Let's Encrypt 仍会访问 80 端口，请将外部 80 端口转发到 ${WebPort} 以完成验证。 |
| 709 | `Required PostgreSQL major version (empty = any):` | 所需 PostgreSQL 主版本（留空=任意）： |
| 710 | `Reset Settings` | 重置面板设置 |
| 711 | `Reset Username & Password` | 重置用户名和密码 |
| 712 | `Reset Web Base Path` | 重置 Web 根路径 |
| 713 | `Restart` | 重启面板 |
| 714 | `Restart Xray` | 重启 Xray |
| 715 | `Restart signal sent to the panel and xray-core.` | 已向面板和 xray-core 发送重启信号。 |
| 716 | `Restart the panel` | 重启面板 |
| 717 | `Restart the panel, Attention: Restarting the panel will also restart xray` | 重启面板，注意：重启面板同时会重启 xray |
| 718 | `Restart xray core` | 重启 xray 内核 |
| 719 | `Restarting panel on PostgreSQL...` | 正在以 PostgreSQL 重启面板... |
| 720 | `Restore failed.` | 恢复失败。 |
| 721 | `Run setup anyway (ensures the xui database/user exist)?` | 仍要执行初始化吗（确保 xui 数据库/用户存在）？ |
| 722 | `SQLite (/etc/x-ui/x-ui.db)` | SQLite（/etc/x-ui/x-ui.db） |
| 723 | `SSH Port Forwarding Management` | SSH 端口转发管理 |
| 724 | `SSL Certificate Management` | SSL 证书管理 |
| 725 | `Select an option (1 or 2):` | 请选择一个选项（1 或 2）： |
| 726 | `Selected rules have been deleted.` | 已删除选中的规则。 |
| 727 | `Server IP detected: ${server_ip}` | 检测到服务器 IP：${server_ip} |
| 728 | `Set 'restart: no' for the container on the host to disable autostart.` | 请在宿主机上将容器设置为 'restart: no' 以关闭开机自启。 |
| 729 | `Set up fail2ban for the panel` | 为面板配置 fail2ban |
| 730 | `Show ban log` | 查看封禁日志 |
| 731 | `Show current settings` | 查看当前配置 |
| 732 | `Show panel status` | 查看面板运行状态 |
| 733 | `Skipping panel path setting.` | 跳过面板证书路径设置。 |
| 734 | `Speedtest by Ookla` | Ookla 测速 |
| 735 | `Standard SSH command:` | 标准 SSH 命令： |
| 736 | `Start` | 启动面板 |
| 737 | `Start automatically: ${green}Managed by Docker${plain}` | 开机自启：${green}由 Docker 管理${plain} |
| 738 | `Start automatically: ${green}Yes${plain}` | 开机自启：${green}是${plain} |
| 739 | `Start automatically: ${red}No${plain}` | 开机自启：${red}否${plain} |
| 740 | `Start the panel` | 启动面板 |
| 741 | `Started` | 已启动 |
| 742 | `Starting automatic SSL certificate generation for server IP...` | 正在为服务器 IP 自动申请 SSL 证书... |
| 743 | `Status: active` | 状态：已启用 |
| 744 | `Stop` | 停止面板 |
| 745 | `Stop the panel` | 停止面板 |
| 746 | `Stop the panel first (x-ui stop) or choose a different output path.` | 请先停止面板（x-ui stop），或选择其他输出路径。 |
| 747 | `Stopping panel to take a consistent snapshot...` | 正在停止面板以获取一致性快照... |
| 748 | `The OS release is: $release` | 系统发行版：$release |
| 749 | `The certificate is installed and auto-renewal is turned on. Specific information is as follows:` | 证书已安装并已开启自动续期，详细信息如下： |
| 750 | `The port is set, Please restart the panel now, and use the new port ${green}${port}${plain} to access web panel` | 端口已设置，请立即重启面板，并使用新端口 ${green}${port}${plain} 访问 Web 面板 |
| 751 | `The rest of the hardening is in force. Upgrade systemd to apply the above.` | 其余加固配置已生效。升级 systemd 后可应用上述配置。 |
| 752 | `There is no service to enable inside the container.` | 容器内没有可设置自启的服务。 |
| 753 | `This command will run on every certificate issue and renew.` | 该命令将在每次签发和续期证书时执行。 |
| 754 | `This function will update all x-ui components to the latest version, and the data will not be lost. Do you want to continue?` | 此功能会将所有 x-ui 组件更新到最新版本，数据不会丢失。是否继续？ |
| 755 | `This function will update the menu to the latest changes.` | 此功能会将管理菜单更新到最新版本。 |
| 756 | `This will obtain a certificate for your server's IP using the shortlived profile.` | 将使用 shortlived 配置为您的服务器 IP 申请证书。 |
| 757 | `This will update x-ui to the latest DEV commit (the rolling 'dev-latest' build, not a stable release). Your data is preserved. Continue?` | 此操作会把 x-ui 更新到最新的开发版提交（滚动更新的 dev-latest 构建，非稳定版）。您的数据会保留。是否继续？ |
| 758 | `This x-ui build does not support .db <-> .dump conversion yet.` | 此版本的 x-ui 尚不支持 .db <-> .dump 转换。 |
| 759 | `To stop it, stop the container from the host:` | 如需停止，请在宿主机上停止容器： |
| 760 | `Two factor authentication has been disabled.` | 双重认证已关闭。 |
| 761 | `Uninstall` | 卸载面板 |
| 762 | `Uninstall the panel` | 卸载面板 |
| 763 | `Uninstalled Successfully.\` | 卸载成功。\ |
| 764 | `Uninstalled Successfully.` | 卸载成功。 |
| 765 | `Unsupported OS '${release}'; install the PostgreSQL client tools manually.` | 不支持的操作系统 '${release}'，请手动安装 PostgreSQL 客户端工具。 |
| 766 | `Unsupported OS for automatic socat installation` | 当前系统不支持自动安装 socat |
| 767 | `Unsupported distro for automatic PostgreSQL purge: ${release}. Remove it manually.` | 当前发行版不支持自动清除 PostgreSQL：${release}，请手动移除。 |
| 768 | `Update` | 更新面板 |
| 769 | `Update Geo Files` | 更新 Geo 规则文件 |
| 770 | `Update Menu` | 更新管理菜单 |
| 771 | `Update geoip/geosite data files` | 更新 geoip/geosite 数据文件 |
| 772 | `Update is complete, Panel has automatically restarted` | 更新完成，面板已自动重启 |
| 773 | `Update panel to the latest dev build` | 更新面板到最新开发版 |
| 774 | `Update panel to the latest stable release` | 更新面板到最新稳定版 |
| 775 | `Update successful. The panel has automatically restarted.` | 更新成功，面板已自动重启。 |
| 776 | `Update the panel first (x-ui update) to a version with 'migrate-db --dump/--restore'.` | 请先将面板更新（x-ui update）到支持 'migrate-db --dump/--restore' 的版本。 |
| 777 | `Update to Dev Channel (latest commit)` | 更新到开发通道（最新提交） |
| 778 | `Upgrade script succeeded, Please rerun the script` | 脚本升级成功，请重新运行本脚本 |
| 779 | `Usage: ${green}x-ui migrateDB [file.db\|file.dump] [output]${plain}` | 用法：${green}x-ui migrateDB [file.db\|file.dump] [output]${plain} |
| 780 | `Using Let's Encrypt shortlived profile (~6 days validity, auto-renews)` | 使用 Let's Encrypt shortlived 配置（约 6 天有效，自动续期） |
| 781 | `Using existing certificate, installing certificates...` | 使用已有证书，正在安装证书... |
| 782 | `Using port ${WebPort} to issue certificate for IP: ${server_ip}` | 使用端口 ${WebPort} 为 IP ${server_ip} 申请证书 |
| 783 | `View Current Settings` | 查看当前配置 |
| 784 | `Warning: these folders contain whitespace and were left out of` | 警告：以下目录路径包含空白字符，已被排除在 |
| 785 | `Web base path has been reset to: ${green}${config_webBasePath}${plain}` | Web 根路径已重置为：${green}${config_webBasePath}${plain} |
| 786 | `Will use port: ${WebPort} to issue certificates. Please make sure this port is open.` | 将使用端口 ${WebPort} 签发证书，请确保该端口已开放。 |
| 787 | `Would you like to customize the Panel Port settings? (If not, a random port will be applied) [y/n]:` | 是否自定义面板端口？（否则将使用随机端口）[y/n]： |
| 788 | `Would you like to modify --reloadcmd for ACME? (y/n):` | 是否修改 ACME 的 --reloadcmd？(y/n)： |
| 789 | `Would you like to set this certificate for the panel? (y/n):` | 是否将此证书应用到面板？(y/n)： |
| 790 | `Wrote database settings to $(xui_env_file_path) (XUI_DB_TYPE=postgres).` | 数据库设置已写入 $(xui_env_file_path)（XUI_DB_TYPE=postgres）。 |
| 791 | `Your domain is ready for issuing certificates now...` | 您的域名已就绪，可以签发证书了... |
| 792 | `Your domain is: ${domain}, checking it...` | 您的域名是：${domain}，正在检查... |
| 793 | `Your domain name is set to: ${CF_Domain}` | 您的域名已设置为：${CF_Domain} |
| 794 | `Your input ${WebPort} is invalid, will use default port 80.` | 您输入的 ${WebPort} 无效，将使用默认端口 80。 |
| 795 | `Your reloadcmd is: ${reloadCmd}` | 您的 reloadcmd 为：${reloadCmd} |
| 796 | `\ After connecting, access the panel at:` | \ 连接成功后，可通过以下地址访问面板： |
| 797 | `\ Choose an option:` | \ 请选择一个选项： |
| 798 | `\ If using SSH key:` | \ 如使用 SSH 密钥： |
| 799 | `\ No listenIP configured. Choose an option:` | \ 未配置 listenIP，请选择一个选项： |
| 800 | `${green}Current SSH Port Forwarding Configuration:${plain}` | ${green}当前 SSH 端口转发配置：${plain} |
| 801 | `${green}Current jail status:${plain}` | ${green}当前 jail 状态：${plain} |
| 802 | `${green}SSH Port Forwarding Configuration:${plain}` | ${green}SSH 端口转发配置：${plain} |
| 803 | `${green} 1.${plain} Install Fail2ban and configure IP Limit` | ${green} 1.${plain} 安装 Fail2ban 并配置 IP 限制 |
| 804 | `${green} 1.${plain} Preset: systemctl reload nginx ; systemctl restart x-ui` | ${green} 1.${plain} 预设：systemctl reload nginx ; systemctl restart x-ui |
| 805 | `${red}Warning: No Cert and Key found! The panel is not secure.${plain}` | ${red}警告：未找到证书和私钥！面板连接不安全。${plain} |
| 806 | `After connecting, access the panel at:` | 连接后，通过以下地址访问面板： |
| 807 | `Choose an option:` | 请选择一个选项： |
| 808 | `If using SSH key:` | 如使用 SSH 密钥： |
| 809 | `No listenIP configured. Choose an option:` | 未配置监听 IP。请选择一个选项： |
| 810 | `Certificate Path: ${cert_path}` | 证书路径：${cert_path} |
| 811 | `Private Key Path: ${key_path}` | 私钥路径：${key_path} |
| 812 | `acme.sh could not be found. Installing now...` | 未找到 acme.sh，正在安装... |
| 813 | `acme.sh could not be found. We will install it.` | 未找到 acme.sh，将自动安装。 |
| 814 | `acme.sh could not be found. we will install it` | 未找到 acme.sh，将自动安装 |
| 815 | `acme.sh is already installed.` | acme.sh 已安装。 |
| 816 | `acme.sh not found, installing...` | 未找到 acme.sh，正在安装... |
| 817 | `chocolate4u datasets` | chocolate4u 数据集 |
| 818 | `detached_x-ui.sh` | out_x-ui.sh |
| 819 | `echo && read -rp "$1 [Default $2]: " temp` | echo && read -rp "$1 [默认 $2]：" temp |
| 820 | `echo -e " ${blue}sudo -u postgres psql -d ${PG_DB}${plain} (as the postgres superuser)"` | echo -e " ${blue}sudo -u postgres psql -d ${PG_DB}${plain} （以 postgres 超级用户执行）" |
| 821 | `echo -e "${green} Database Selection ${plain}"` | echo -e "${green} 数据库选择 ${plain}" |
| 822 | `echo -e "${green}\ 2.${plain} Input your own command"` | echo -e "${green}\ 2.${plain} 手动输入自定义命令" |
| 823 | `echo -n -e "${yellow}Press enter to return to the main menu: ${plain}"` | echo -n -e "${yellow}按回车返回主菜单：${plain}" |
| 824 | `failed` | 失败 |
| 825 | `failed to open <file>: no such file or directory` | 无法打开 <文件>：文件或目录不存在 |
| 826 | `geo files` | Geo 文件 |
| 827 | `get current settings error, please check logs` | 获取当前设置失败，请查看日志 |
| 828 | `install acme failed, please check logs` | 安装 acme 失败，请查看日志 |
| 829 | `install socat failed, please check logs` | 安装 socat 失败，请查看日志 |
| 830 | `install socat succeed...` | socat 安装成功... |
| 831 | `mtproto inbound ${id} (${bind}): ${green}Running${plain}` | MTProto 入站 ${id} (${bind})：${green}运行中${plain} |
| 832 | `mtproto inbound ${id} (${bind}): ${red}Not Running${plain}` | MTProto 入站 ${id} (${bind})：${red}未运行${plain} |
| 833 | `panel Failed to start, Probably because it takes longer than two seconds to start, Please check the log information later` | 面板启动失败，可能启动耗时超过两秒，请稍后查看日志 |
| 834 | `pg_dump/pg_restore are still unavailable after installation.` | 安装后 pg_dump/pg_restore 仍不可用。 |
| 835 | `postgresql${want} is not in the enabled repositories; adding the official PostgreSQL yum repository...` | 已启用的软件源中没有 postgresql${want}，正在添加 PostgreSQL 官方 yum 源... |
| 836 | `postgresql-client-${want} is not in the distribution repositories; adding the official PostgreSQL apt repository...` | 发行版软件源中没有 postgresql-client-${want}，正在添加 PostgreSQL 官方 apt 源... |
| 837 | `prompt text` | 提示文本 |
| 838 | `read -rp "$1 [y/n]: " temp` | read -rp "$1 [y/n]：" temp |
| 839 | `runetfreedom datasets` | runetfreedom 数据集 |
| 840 | `success` | 成功 |
| 841 | `this machine, including any used by other applications. This cannot be undone.` | 包括其他应用正在使用的数据库，此操作不可撤销。 |
| 842 | `ufw firewall is already installed` | ufw 防火墙已安装 |
| 843 | `ufw firewall is not installed. Installing now...` | 未安装 ufw 防火墙，正在安装... |
| 844 | `x-ui Autostart Cancelled successfully` | x-ui 已成功取消开机自启 |
| 845 | `x-ui Failed to cancel autostart` | x-ui 取消开机自启失败 |
| 846 | `x-ui Failed to set Autostart` | x-ui 设置开机自启失败 |
| 847 | `x-ui Set to boot automatically on startup successfully` | x-ui 已成功设置为开机自启 |
| 848 | `x-ui Started Successfully` | x-ui 启动成功 |
| 849 | `x-ui and xray Restarted successfully` | x-ui 与 xray 重启成功 |
| 850 | `x-ui and xray stopped successfully` | x-ui 与 xray 已成功停止 |
| 851 | `x-ui binary not found at ${bin}. Is the panel installed?` | 未在 ${bin} 找到 x-ui 二进制文件，面板是否已安装？ |
| 852 | `x-ui control menu usages (subcommands):` | x-ui 管理菜单用法（子命令）： |
| 853 | `x-ui is not installed.` | x-ui 未安装。 |
| 854 | `xray state: ${green}Running${plain}` | xray 状态：${green}运行中${plain} |
| 855 | `xray state: ${red}Not Running${plain}` | xray 状态：${red}未运行${plain} |
| 856 | `xray-core Restart signal sent successfully, Please check the log information to confirm whether xray restarted successfully` | 已成功发送 xray-core 重启信号，请查看日志确认 xray 是否重启成功 |
