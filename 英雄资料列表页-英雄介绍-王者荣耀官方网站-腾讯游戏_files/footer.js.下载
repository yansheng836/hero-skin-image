
/**
 * pvp Footer JS
 * Author: sonichuang
 * Create: 2017-05-31
 */
var pvpFooter = (function(){
	var util = {},
		fn = {},
		$footer = "",
		init = function(){};

	fn = {
		jsLoader: function(url, callback, options) {
			options = options || {};
			var head = document.getElementsByTagName('head')[0] || document.documentElement,
				script = document.createElement('script'),
				done = false;
			script.src = url;
			if (options.charset) {controller
				script.charset = options.charset;
			}
			script.onerror = script.onload = script.onreadystatechange = function() {
				if (!done && (!this.readyState || this.readyState == "loaded" || this.readyState == "complete")) {
					done = true;
					if (callback) {
						callback();
					}
					script.onerror = script.onload = script.onreadystatechange = null;
					head.removeChild(script);
				}
			};
			head.insertBefore(script, head.firstChild);
		}
	};

	util.addFooterCSS = function(){
		var footerCSS = '';
			footerCSS += '.footer-wrap{position:relative;z-index:2;height:362px;background:url(//game.gtimg.cn/images/yxzj/web201605/top_banner/bg_footer.jpg) no-repeat center 0;}';
			footerCSS += '.footer-wrap p,.footer-wrap .foot_links li{margin:0;font-size:12px;}';
			footerCSS += '.footer-wrap .foot{position: relative;background:none;width:1200px;padding-top:80px;}';
			footerCSS += '.footer-wrap .foot_lefts{display: block;float:none;height: 66px;padding-bottom:10px;margin-bottom:32px;border-bottom:2px solid #d4d4d4;}';
			footerCSS += '.footer-wrap .foot_cpright{padding:0;}';
			footerCSS += '.footer-wrap .foot_ieg_logo{width:285px;height:64px;margin:0;background: url(//game.gtimg.cn/images/yxzj/web201605/main/spr.png) no-repeat;}';
			footerCSS += '.footer-wrap .logo1{width:70px;height:64px;margin:0;background: url(//game.gtimg.cn/images/yxzj/web201605/main/spr.png) no-repeat -285px 0;}';
			footerCSS += '.footer-wrap .logo2,.footer-wrap .limit_age{display: none;}';
			footerCSS += '.footer-wrap .foot_links,.footer-wrap .foot_links a:link,.footer-wrap .foot_links a:visited{color:#646467;text-decoration: none;}';
			footerCSS += '.footer-wrap .foot_links{position: relative;margin:0;width:650px;}';
			footerCSS += '.footer-wrap .copyright_en{padding-top:6px;}';
			footerCSS += '.footer-wrap .copyright_zh{position: absolute;right:0;top:26px;}';
			footerCSS += '.footer-wrap .foot-tips{position: absolute;left:0;top:170px;padding-top:0;width:508px;font-size: 12px;color: #666;}';
			footerCSS += '.footer-wrap .foot-tips .fb{color: #333;font-weight: bold;}';
			footerCSS += '.footer-wrap .foot-tips em{font-style:normal;margin-right:12px;color:#6d6d6d;}';
			footerCSS += '.footer-wrap .foot-tips .intro{margin-top:6px;}';
			footerCSS += '.footer-wrap .foot-tips .report{position: absolute;left:550px;top:106px;width: 300px;}';	
		
		if(document.all){ // document.createStyleSheet(url)
	        document.createStyleSheet().cssText = footerCSS
	    }else{ 			 //document.createElement(style)
	        var fCSS = document.createElement('style'); 
	        fCSS.innerHTML=footerCSS; 
	        document.head.appendChild(fCSS);
	    }
	}

	util.addFooterHTML = function(){
		var footerHTML = '';
			footerHTML += '<div id="gfooter" ams="15592/35033/m11738" age="17" ieg-logo="1" class="footer-wrap">';
			footerHTML += '    <a target="_blank" href="//timi.qq.com/" title="天美工作室群" class="foot_left logo1">timi</a>';
			footerHTML += '    <div class="foot_bottom foot-tips fl">';
			footerHTML += '    	<p class="fb">温馨提示：本游戏适合16岁(含)以上玩家娱乐</p>';
			footerHTML += '    	<p><em>抵制不良游戏</em><em>拒绝盗版游戏</em><em>注意自我保护</em><em>谨防受骗上当</em><em>适度游戏益脑</em><em>沉迷游戏伤身</em><em>合理安排时间</em><em>享受健康生活</em></p>        <p class="intro">《王者荣耀》全部背景故事发生于架空世界“王者大陆”中。相关人物、地理、事件均为艺术创作，并非正史。若因观看王者故事对相关历史人物产生兴趣，建议查阅正史记载。</p>';
			footerHTML += '    	<p class="report">全国文化市场统一举报电话：12318</p>';
			footerHTML += '    </div>';
			footerHTML += '</div>';
		var fDiv = document.createElement('div');
			fDiv.innerHTML = footerHTML;
		document.getElementsByTagName("body")[0].appendChild(fDiv);
	};
	init = function(){
		util.addFooterCSS();
		util.addFooterHTML();
		fn.jsLoader("//game.gtimg.cn/images/js/2018foot/foot.js");
	};
	return{
		init : init
	}
})()
pvpFooter.init();
