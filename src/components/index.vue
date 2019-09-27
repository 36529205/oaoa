<template>
  <div>
    <!-- header start-->
    <header>
      <div class="w">
        <a href="#">
          <img src="@/assets/images/header.jpg" >
        </a>
      </div>
    </header>
    <nav class="shortcut">
      <div class="w">
        <ul>
          <li>
            <a href="#"><i class="f10"></i> 北京</a>           
          </li>
          <li>
            
            <a href="#">您好，请登录</a>
            <a herf="#">免费注册</a>
          </li>
          <li>
              <a herf="#">我的订单</a>
          </li>
          <li>
            
            <a href="#">我的京东<i></i></a>
          </li>
          <li>
            
            <a href="#">京东会员</a>
          </li>
          <li>
            
            <a href="#">企业采购</a>
          </li>
          <li>
            
            <a href="#">客服服务<i></i></a>
          </li>
          <li>
            
            <a href="#">网页导航<i></i></a>
          </li>
          <li class="mobile">
            
            <a href="#">
                手机京东
            </a>
            <img src="../assets/images/mobile.png" alt="">
          </li>
        </ul>
      </div>
    </nav>
    <div class="w middle">

        <!-- jd logo-->
        <div class="log">
            <h1>
                <a href="#"></a>
            </h1>
        </div>

        <!-- search bar -->
        <div class="search">
            <input placeholder="饮水机 立式"/>
            <button ><i> </i></button>
        </div>

        <!-- Shopping cart -->
            <a class="shoppingCart">
                <i></i>
                <span>购物车</span>
                <span>0</span>
            </a>

        <!-- key -->
        <div class="key">
            <ul  >
                <li v-for="(item,index) in list" :key="index" ><a ref="#">{{ item.name}}</a></li>
            </ul>   
        </div>

        <!--  navKey -->
        <div class="navKey">
            <ul >
                <li v-for="(item,index) in list2" :key="index"><a ref="#"> {{item.name}}</a></li>
            </ul>
        </div>

        <!-- super -->
        <div class="super">
            <a ref="#"></a>
        </div>
    </div>
    <!-- middleNav -->
    <div class="w middleNav">
      <div class="middle_nav_l"> 
        <ul>
          <ul>
            <li v-for="item in middleNav" :key="item.id" >
              <a v-for="items  in item.value" :key="items" href="#">
                {{items}}
              </a>
            </li>
          </ul>
        </ul>
        <div class="left_ad">
          <a herf="#"></a>        
        </div>
      </div>
      <div class="middle_nav_m"> 
        <div class="top">
          <a href="#"><img src="../assets/images/ad-r.jpg" width="791px" height="340px" alt=""/></a>
        </div>
        <div class="bottom_l">
          <a href="#"><img src="../assets/images/l.jpg" width="390px" height="130px" alt=""/></a>
        </div>
        <div class="bottom_r">
          <a href="#"><img src="../assets/images/r.jpg" width="390px" height="130px" alt=""/></a>
        </div>
      </div>
      <div class="middle_nav_r"> 
        <div class="r_top">
          <div class="r_top_head">
              <div class="title">Hi,欢迎来到京  东</div>
              <div><a ref="load" href="#">登录</a> <a ref="regist" href="#">注册</a>  </div>
          </div>
          <div class="button">
              <a href="#" class="button_l">新人福利</a>
              <a href="#" class="button_r">PLUS会员</a>
          </div>
          <div class="content">
        </div>
        </div>
        <div class="r_center">
           <div class="r_c_nav">
             <input class="button_r_b b_61" type="button" value="促销"/>
             <input class="button_r_b p_l_16" type="button" value="公告"/>
             <a href="#" class="r_c_more">更多</a>
           </div>
           <div class="r_c_ad">
             <ul>
               <li><a href="#">飘柔 挑战3天不洗头</a></li>
               <li><a href="#">AMD锐龙Ryzen3首发</a></li>
               <li><a href="#">家具狂欢领券199减100</a></li>
               <li><a href="#">益生菌领券满399减100</a></li>
             </ul>
           </div>
          </div>
        
        <div class="r_bottom">
          <div class="box">
          <ul>
            <li><div class="bc"></div><a>话费</a></li>
            <li><div class="bc"></div><a>机票</a></li>
            <li><div class="bc"></div><a>酒店</a></li>
            <li><div class="bc"></div><a>游戏</a></li>
          </ul>
          <ul>
            <li><div class="bc"></div><a>企业购</a></li>
            <li><div class="bc"></div><a>加油卡</a></li>
            <li><div class="bc"></div><a>电影票</a></li>
            <li><div class="bc"></div><a>火车票</a></li>
          </ul>
          <ul>
            <li><div class="bc"></div><a>众筹</a></li>
            <li><div class="bc"></div><a>理财</a></li>
            <li><div class="bc"></div><a>礼品卡</a></li>
            <li><div class="bc"></div><a>白条</a></li>
          </ul>
          </div>
        </div>
      </div>
    </div>
    <!-- footer -->
    <footer>

          <!-- footer first line -->
            <div class="footerTop">
                <ul class="w footerTop-title">
                    <li>
                        <h5></h5>
                        <span>品类齐全，轻松购物</span>
                    </li>
                    <li>
                        <h5></h5>
                        <span>多仓直发，极速配送</span>
                    </li>
                    <li>
                        <h5></h5>
                        <span>正品行货，精致服务</span>
                    </li>
                    <li>
                        <h5></h5>
                        <span>天天低价，畅选无忧</span>
                    </li>
                </ul>
            </div>
            <!-- footerHelp -->
            <div class=" w footerHelp">
              <dl>
                <dt><a>购物指南</a></dt>
                <dd><a>购物流程</a></dd>
                <dd><a>会员介绍</a></dd>
                <dd><a>生活旅行</a></dd>
                <dd><a>常见问题</a></dd>
                <dd><a>大家电</a></dd>
                <dd><a>联系客服</a></dd>
              </dl>
             <dl>
                <dt><a>配送方式</a></dt>
                <dd><a>上门自提</a></dd>
                <dd><a>211限时达</a></dd>
                <dd><a>配送服务查询</a></dd>
                <dd><a>配送费用收取标准</a></dd>
                <dd><a>海外配送</a></dd>
              </dl>
              <dl>
                <dt><a>支付方式</a></dt>
                <dd><a>货到付款</a></dd>
                <dd><a>在线支付</a></dd>
                <dd><a>分期付款</a></dd>
                <dd><a>邮局汇款</a></dd>
                <dd><a>公司转账</a></dd>
              </dl>
              <dl>
                <dt><a>售后服务</a></dt>
                <dd><a>售后政策</a></dd>
                <dd><a>价格保护</a></dd>
                <dd><a>退款说明</a></dd>
                <dd><a>返修/退换货</a></dd>
                <dd><a>取消订单</a></dd>
              </dl>
              <dl>
                <dt><a>特色服务</a></dt>
                <dd><a>夺宝岛</a></dd>
                <dd><a>DIY装机</a></dd>
                <dd><a>延保服务</a></dd>
                <dd><a>京东E卡</a></dd>
                <dd><a>京东通信</a></dd>
                <dd><a>京东JD+</a></dd>
              </dl>
              <dl>
                <dt>京东自营覆盖区县</dt>
                <dd>京东已向全国2661个区县提供自<br/>营配送服务，支持货到付款、POS<br/>机刷卡和售后上门服务。
                <div><a href="#">查看详情></a></div>
                </dd>
              </dl>
            </div>

            <div class="w footerBottom">
              <div class="footerNav">
                <a href="#">关于我们</a>
                <a href="#">联系我们</a>
                <a href="#">联系客服</a>
                <a href="#">合作招商</a>
                <a href="#">商家帮助</a>
                <a href="#">营销中心</a>
                <a href="#">手机京东</a>
                <a href="#">友情链接</a>
                <a href="#">销售联盟</a>
                <a href="#">京东社区</a>
                <a href="#">风险监测</a>
                <a href="#">隐私政策</a>
                <a href="#">京东公益</a>
                <a href="#">English</a>
                <a href="#">Site</a>
                <a href="">Media & IR</a>
              </div>
              
              <div class="footerCenter">
                <span>
                  <a href="#">京公网安备 11000002000088号</a>
                  <a href="#">京ICP证070359号</a>
                  <a href="#">互联网药品信息服务资格证编号(京)-经营性-2014-0008</a>
                  <a href="#">新出发京零 字第大120007号</a><br/>
                </span>
                <span>
                  <a href="#">互联网出版许可证编号新出网证(京)字150号</a>
                  <a href="#">出版物经营许可证</a>
                  <a href="#">网络文化经营许可证京网文[2014]2148-348号</a>
                  <a href="#">违法和不良信息举报电话：4006561155</a><br/>
                </span>
                <span>
                  <a href="#">Copyright © 2004 - 2019 京东JD.com 版权所有</a>
                  <a href="#">消费者维权热线：4006067733 经营证照</a>
                  <a href="#"> (京)网械平台备字(2018)第00003号 </a>
                  <a href="#">营业执照</a><br/>
                </span>
                <span>
                  <a href="#">京东旗下网站： 京东钱包</a>
                  <a href="#">京东云</a>
                </span>
              </div>
              <div class="copyright">
                <a href="#"></a>
                <a href="#"></a>
                <a href="#"></a> 
                <a href="#"></a>
                <a href="#"></a>
                <a href="#"></a>
              </div>
            </div>
    </footer>
  </div>
</template>
<script>
export default {
    data(){
        return{
            list:[
               { name:'魅族Pro7'},
               { name:'机械革命'},
               { name:'园艺肥'},
               { name:'6折清仓'},
               { name:'抽奖赢空调'},
               { name:'荣耀6x'},
               { name:'折叠床'},
               { name:'京东超市'},
               { name:'手套'},
            ],
            list2:[
                {name:"秒杀"},
                {name:"优惠券"},
                {name:"闪购"},
                {name:"拍卖 "},
                {name:"服装城"},
                {name:"京东超市"},
                {name:"生鲜"},
                {name:"全球购"},
                {name:"京东金融"},
            ],
            middleNav:[
              {
                id: 1,
                value:[
                  '家用电器'
                  ]
              },
              {
                id: 2,
                value:['手机','运营商','数码']
              },
              {
                id: 3,
                value:['电脑','办公']
              },
              {
                id: 4,
                value:['家具','家居','家装','厨具']
              },
              {
                id: 5,
                value:['男装','女装','童装','内衣']
              },
              {
                id: 6,
                value:['美妆个护','宠物',]
              },
              {
                id: 7,
                value:['女鞋','箱包','钟表','珠宝']
              },
              {
                id: 8,
                value:['男鞋','运动','户外']
              },
              {
                id: 9,
                value:['汽车','汽车用品']
              },
              {
                id: 10,
                value:['母婴','玩具乐器']
              },
              {
                id: 11,
                value:['食品','酒类','生鲜','特产']
              },
              {
                id: 12,
                value:['礼包鲜花','农资绿植']
              },
              {
                id: 13,
                value:['医药保健','计生情趣']
              },
              {
                id: 14,
                value:['图书','音像','电子书']
              },
              {
                id: 15,
                value:['机票','酒店','旅游','生活']
              },
              {
                id: 16,
                value:['理财','众筹','白条','保险']
              },
            ]
        }
    },
    methods:{

    },

};
</script>
<style>
.top {
  background-color: #000000;
}
.shortcut {
  background: #e3e4e5;
  border-bottom: 1px solid #dddddd;
}
</style>