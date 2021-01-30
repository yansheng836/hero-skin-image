(function() {
	var Cookie = {};
	Cookie.get = function(sName,sDefaultValue){var sRE = "(?:; |^)" + sName + "=([^;]*);?";var oRE = new RegExp(sRE);if (oRE.test(document.cookie)) {return unescape(RegExp["$1"]);} else {return sDefaultValue||null;}};
	Cookie.set = function(sName,sValue,iExpireSec,sDomain,sPath,bSecure){if(!sName){return;}if(!sValue){sValue = "";}var str = sName + "=" + escape(sValue) + "; ";if(!isNaN(iExpireSec)){var oDate = new Date();oDate.setTime(oDate.getTime() + iExpireSec*1000);str += "expires=" + oDate.toGMTString() + "; ";}if(sDomain){str += "domain=" + sDomain + "; ";}if(sPath){str += "path=" + sPath + "; ";}else{str += "path=/; ";}if(bSecure){str += "secure";}document.cookie = str;};
	
	/*生成32位随机数*/
	function getRandomStr() {
		var data = [];
		for (var i = 0; i < 10; i++)
			data.push(i);
			
		var str = "a";
		var begin = str.charCodeAt();
		for (var i = 0; i < 26; i++)
			data.push(String.fromCharCode(begin + i));
		
		str = "A";
		begin = str.charCodeAt();
		for (var i = 0; i < 26; i++)
			data.push(String.fromCharCode(begin + i));			
			
		str = "";
		for (var i = 0; i < 32; i++)
			str += data[Math.floor(Math.random() * 62)];
		
		return str;
	}
	
	/*往Cookie种下随机数作为用户id*/
	var name = "ieg_ingame_userid";
	if (!Cookie.get(name, ""))
		Cookie.set(name, getRandomStr(), 86400);

	/*上报PV、UV*/
	var date = new Date();
	var year = date.getFullYear();
	var month = date.getMonth() + 1;
	var day = date.getDate();
	date = "" + year + (month < 10 ? "0" + month : month) + (day < 10 ? "0" + day : day);
	var url = location.host + location.pathname; /*url中不带参数*/
	var request = document.createElement("script");
	request.src = "https://lotus.ingame.qq.com/tdbank/report?r=" + Math.random() + "&params=" + Cookie.get(name, "") + "|" + date + "|" + url;
	(document.body || document.getElementsByTagName("head")[0]).appendChild(request);
})();/*  |xGv00|49972fd06ff5fe3d9f6a7a87f7f41196 */