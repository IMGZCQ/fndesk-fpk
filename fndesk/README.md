# <span style="color:#ff6b6b">fndesk</span> 飞牛桌面管理工具

<div style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 20px; border-radius: 10px; color: white; margin: 20px 0;">
  <h2 style="margin-top: 0;">实在太强大！</h2>
  <p style="font-size: 18px; margin-bottom: 0;">我的飞牛我做主,多处自定样式主题美化,桌面图标任君摆布,让飞牛成为你的导航页，收藏夹,Docker应用入口</p>
</div>

## <span style="color:#4ecdc4">主要功能</span>
* ✨ 实现图标，文件夹自由，彻底取代收藏夹  
🌈智能识别内外网环境，更多自定义链接  
🌐 飞牛桌面内文件夹自由拖动调整大小  
🖼️ 文件夹和图标图片完全自由设置  
👑 更多个性化设置：背景，LOGO，标题等  
⚙️ 多层文件夹，右键菜单，拓展更多功能  

## <span style="color:#4ecdc4">使用说明</span>
* 🍭 有兴趣的灵魂请加入Q群组1039270739参与讨论  
  本工具是一个单纯的修改工具,修改配置生效后可以停用甚至卸载本工具,重启也能一直生效
  
* 🥕 本工具有飞牛应用Fpk版和Docker版,选其一安装就可以,不建议同时安装！
  
* 🍔 大致使用流程：修改操作>保存配置>立即生效(>清理缓存)  
  (保存和生效是分开, 配置保存后, 就算还原或系统升级,只要重新保存应用即可)

* 🍟 配置文件都在deskdata目录里, 要备份还原移植配置都可以的。  
  (Docker Compose的配置目录在Compose文件同在的目录下,  
  飞牛应用中心安装的配置文件在[文件管理]>应用文件>fndesk目录里)

* 🥤 不生效? 99%的不生效都是缓存造成的, 清理缓存和强制刷新(Ctrl+F5)不太好使  
  建议用浏览器的无痕模式, 或者按F12进入开发者模式到 网络 里把 禁用缓存 勾选上

* 🍦 忘记密码?  
  只需删除deskdata目录里面的pw.json文件即可访问时重新初始化密码

* 🧀 启用HTTPS?
  把证书放在deskdata/ssl目录(server.crt和server.key) 然后重启程序即可

## <span style="color:#118ab2">使用方法(2选1)</span>

<div style="background-color: #e6f7ff; padding: 20px; border-radius: 10px; margin-bottom: 20px;">
   <h4 style="margin-top: 0;">1.新手推荐:下载飞牛应用安装包,到应用中心左下角手动安装：</h4>
  
  [fpk下载链接](https://fndesk.imcq.top/?url=dl&at=GitHUb "点击我没错了")
  
  <h4 style="margin-top: 0;">2.玩家可用:在飞牛Docker compose粘贴以下代码：</h4>
  
  <div style="background-color: #1e293b; color: #e2e8f0; padding: 15px; border-radius: 8px; overflow-x: auto;">
    <pre><code>services:
  fndesk:                    #Compose项目名称
    container_name: fndesk        #docker容器名称
    image: imgzcq/fndesk:latest    #镜像名称
    ports:
     - 9990:9990              #冒号左边修改自定义端口
     - 9991:9991              # HTTPS端口 
    volumes:
     - /usr/trim/www:/fnw        #不能改！
     - /usr/trim/share/.restore:/res #不能改！
     - /usr/local/apps/@appcenter/trim.media:/trim.media
      # ↑ v0.73起开放影视个性化需加入此项
     - ./deskdata:/deskdata       #冒号左边的可以改但不建议     
    restart: always             #容器自动启动应用配置  </code></pre>
    跑码完成访问9990端口即可
  </div>
</div>
  
## <span style="color:#7209b7">效果展示</span>

**文件夹自由拖放，自由缩放，双击最大化**

<img src="https://github.com/user-attachments/assets/e6b4f731-51f2-412c-b5e7-a2e253ad3032" alt="fn-icon界面展示4" style="width: 480px; height: auto;">

**识别内外网连接，3个自定义连接，支持多层文件夹**

<img src="https://github.com/user-attachments/assets/b4d8395f-1f2e-493c-a214-ccafdbcdbdc1" alt="fn-icon界面展示4" style="width: 480px; height: auto;">

**效果预览**
<img width="1679" height="865" alt="98c1d486d22f1fddc5f8ef51bf1f7768" src="https://github.com/user-attachments/assets/4ce0ed0a-abe4-43da-8dbc-4f6841f4bf81" />
<img width="933" height="1057" alt="image" src="https://github.com/user-attachments/assets/0bb969ab-f0e1-4eda-8ec0-3cda466117bf" />
<img width="1061" height="1040" alt="11112" src="https://github.com/user-attachments/assets/ae18d97e-33bf-4c50-8527-77237e61bdf5" />
![H)E}P%(Q1 )4ZKZ{01E35H6](https://github.com/user-attachments/assets/b13f5dfc-1989-413f-b3c1-3c6ccbfba8e1)
<img width="1270" height="992" alt="ScreenShot_2025-10-30_111530_261" src="https://github.com/user-attachments/assets/f84ebfa8-e060-468c-9749-8feac117302b" />
<img width="1051" height="1246" alt="image" src="https://github.com/user-attachments/assets/7ccde508-6035-44a7-8d10-fed973b8ad22" />
<img width="1037" height="1044" alt="1111" src="https://github.com/user-attachments/assets/5cd746cd-345f-4e56-9975-e4b30ea427ed" />
<img width="1001" height="1011" alt="11113" src="https://github.com/user-attachments/assets/7aba2b91-81c9-4651-8b7e-1c3b2d5758f2" />
<img width="855" height="957" alt="ScreenShot_2025-11-12_000235_088" src="https://github.com/user-attachments/assets/73b4a832-aa8d-40f8-9881-0432f8fe78eb" />











