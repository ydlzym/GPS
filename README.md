# GPS
模仿实现雷达扫描，使用UDP实现通信，通信格式：1B通信站编号+GPGGA格式的GPS数据。udp服务器监听2323端口，等待客户端发送数据（server包UDPClinentTest发送测试数据）。基站编号默认为0，经纬度坐标保存在数据库中。udp服务器端将从站编号及经纬度解析后存入数据库。使用html5 的canvas标签实现扫描界面。每隔1s更新一次数据，并将相对位置显示在界面中，同时计算从站距离基站位置和当前速度。界面长1000px,高600px。（另：计算GPS坐标距离公式是参考网上公式，可能有误，请见谅）
