###广播服务接口
> 用于将游戏元数据帧(game meta data frame)添加到Steam广播服务中  
> 接口URL: POST https://partner.steam-api.com/IBroadcastService/PostGameDataFrame/v1/  
  
| 参数名 | 参数类型 | 是否必填 | 描述 |
|:---:|:---:|:---:|:---:|
| key | string | ✔ | Steamworks Web API publisher authentication key.
|appid | uint32 | ✔	 |
|steamid |	uint64	| ✔	
|broadcast_id	| uint64 |	✔	
|frame_data	 |string |	✔	

- 注意这是一个服务接口, 接口调用需要带上input_json作为参数  
  调用需要一个publish API key, 这个接口必须从安全服务器调用,不能从直接从客户端调用