# Angular2-image-not-found-situation
Angular 当src 图片加载失败的处理办法. 


In Angular2 when we use src to load picture , If the img not found we need to do some error image load


In HTML page 
<img src = "someError url link" (error) = "errHandler($event)"/>

In Ts file
make some string to define handler error link:
  public imageErrorHandlerLink = "Https://localhost:somenumber/assets/images/someErrorHandlerImg.png";
make error handler function :
  errHandler(event){event.target.src= imageErrorHandlerLink;}





