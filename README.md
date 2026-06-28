## 前言

随着移动互联网的快速发展，微信小程序凭借其便捷性和普及度成为了众多商家的重要销售渠道。基于此，我们开发了一款基于微信平台的文玩销售小程序SSM，为广大文玩爱好者提供便捷、高效的购物体验。

## 内容介绍

本项目是一款集文玩展示、购买、支付、售后等功能于一体的微信小程序。用户可以在小程序中浏览各种文玩商品，查看详细信息，进行在线购买并完成支付。同时，后台管理系统方便管理员对商品、订单、用户等进行管理，提高运营效率。

## 技术介绍

- 语言：Java
- 使用框架：Spring、Spring MVC、MyBatis、微信小程序
- 前端技术：JS、Vue、CSS3、Uniapp
- 开发工具：IDEA/Eclipse，Uniapp
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven：apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

## 核心代码

以下是项目中的一部分核心代码，展示了如何通过MyBatis实现商品信息的查询：

```java
// Mapper接口
public interface ProductMapper {
    List<Product> queryProductList();
}

// Mapper XML
<select id="queryProductList" resultType="Product">
    SELECT * FROM product
</select>

// Service层
@Service
public class ProductService {
    @Autowired
    private ProductMapper productMapper;

    public List<Product> queryProductList() {
        return productMapper.queryProductList();
    }
}

// Controller层
@RestController
@RequestMapping("/product")
public class ProductController {
    @Autowired
    private ProductService productService;

    @GetMapping("/list")
    public List<Product> productList() {
        return productService.queryProductList();
    }
}
```

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

## 项目截图
![封面图片](https://img11.360buyimg.com/ddimg/jfs/t1/351269/35/3079/116428/68c57e17F391b25ec/d5ee1f928d58d3b6.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/324934/16/19641/33239/68c57defF4f00db76/cbcaa133bb08129f.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/326175/25/19600/64472/68c57defF4fcda045/30ae8ee91c4464da.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/343289/38/2786/24775/68c57defF4c695455/e406ee380e261995.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/327034/33/19755/39718/68c57defFa4dd680d/70875e14e87430ac.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/332878/14/12846/33304/68c57defF8b2a22b7/838bac3f671923f4.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/346753/17/2944/25227/68c57df0Fc29ab770/97d593541510142e.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/332026/4/12846/23068/68c57df0F02cb3dc1/122c1d5f0da20c4f.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/325034/15/19680/10937/68c57df0F59f76130/03f4021c07110db3.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/337415/17/10223/65768/68c57df0Ffc24e26e/89cf7da5d7a2cefa.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
