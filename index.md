---
layout: default
---

# Hi, there.

## I'm Zhou Yang. Welcome to my offical website.

***
<%
Locale locale=request.getLocale();
Calendar calendar=Calendar.getInstance(locale);
int hour=calendar.get(Calendar.HOUR_OF_DAY);
String greeting="";
if(hour<=6){
 greeting="现在是凌晨。";
}else if(hour<=9){
 greeting="早上好！";
}else if(hour<=12){
 greeting="上午好！";
}else if(hour<=18){
 greeting="下午好！";
}else if(hour<=24){
 greeting="晚上好！";
}else{
 greeting="获得时间出错，请调试!";
}
 %>

