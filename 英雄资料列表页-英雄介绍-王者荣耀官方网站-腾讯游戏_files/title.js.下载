!function (t, e) {
  var o = function (t) {
    return e.getElementById(t)
  }
    , n = Math.random()
    , a = "//game.gtimg.cn/"
    , s = a + "images/js/title/"
    , i = navigator.userAgent.indexOf("MSIE") != -1 && !window.XMLHttpRequest
    , l = l || {};
  l = {
    Cookie: {
      get: function (t, o) {
        var n = "(?:; |^)" + t + "=([^;]*);?"
          , a = new RegExp(n);
        return a.test(e.cookie) ? unescape(RegExp.$1) : o || null
      },
      set: function (t, o, n, a, s, i) {
        if (t) {
          o || (o = "");
          var l = t + "=" + escape(o) + "; ";
          if (!isNaN(n)) {
            var r = new Date;
            r.setTime(r.getTime() + 1e3 * n),
              l += "expires=" + r.toGMTString() + "; "
          }
          a && (l += "domain=" + a + "; "),
            l += s ? "path=" + s + "; " : "path=/; ",
            i && (l += "secure"),
            e.cookie = l
        }
      },
      clear: function (t) {
        this.set(t, "", new Date(0), "qq.com", "/")
      }
    },
    loadCSS: function (t) {
      var o = e.createElement("link");
      o.href = t,
        o.rel = "stylesheet",
        o.type = "text/css",
        e.getElementsByTagName("head")[0].appendChild(o)
    },
    loadJS: function (t, o, n) {
      n = n || {};
      var a = e.getElementsByTagName("head")[0] || e.documentElement
        , s = e.createElement("script")
        , i = !1;
      s.src = t,
        n.charset && (s.charset = n.charset),
        s.onerror = s.onload = s.onreadystatechange = function () {
          i || this.readyState && "loaded" != this.readyState && "complete" != this.readyState || (i = !0,
            "function" == typeof o && o(),
            s.onerror = s.onload = s.onreadystatechange = null,
            a.removeChild(s))
        }
        ,
        a.insertBefore(s, a.firstChild)
    },
    eventUtil: {
      addListener: function (t, e, o) {
        t.addEventListener ? t.addEventListener(e, o, !1) : t.attachEvent ? t.attachEvent("on" + e, o) : t["on" + e] = o
      },
      getEvent: function (t) {
        return t || window.event
      },
      getTarget: function (t) {
        return t.target || t.srcElement
      },
      preventDefault: function (t) {
        t.preventDefault ? t.preventDefault() : t.returnValue = !1
      },
      removeListener: function (t, e, o) {
        t.removeEventListener ? t.removeEventListener(e, o, !1) : t.deattachEvent ? t.detachEvent(e, o) : t["on" + e] = null
      },
      stopPropagation: function (t) {
        t.stopPropagation ? t.stopPropagation() : t.cancelBubble = !0
      }
    }
  };
  var r = r || {};
  r = {
    init: function () {
      this.wrap().loadO2Media().footMedia().rankEffct().tgConsole()
    },
    wrap: function () {
      var t = e.createElement("div")
        , o = "?ADTAG=IED.InnerCop.gameWeb.topNav";
      return l.loadCSS(s + "ost.css?ran=" + n, "link"),
        t.className = "ost_box ost_bg",
        t.id = "ost_box",
        t.style.cssText = "position:absolute;",
        t.innerHTML = '<ul class="ost_inner ost_lsn"><li class="ost_logo ost_h40 ost_fl ost_bg"><a rel="noopener" href="//game.qq.com/' + o + '" target="_blank" class="ost_blnk ost_hdn" title="\u817e\u8baf\u6e38\u620flogo">\u817e\u8baf\u6e38\u620flogo</a></li><li id="ost_g" class="ost_ad ost_h40 ost_fl"></li><li class="ost_total ost_ml10 ost_fr"><h3 class="ost_czsh ost_h40" ><a rel="noopener" target="_blank" href="https://game.qq.com/web201910/jiazhang.html?ADTAG=gamepcbanner">\u6210\u957f\u5b88\u62a4\u5e73\u53f0</a></h3><h3 class="ost_title ost_h40" id="ost_t">\u817e\u8baf\u6e38\u620f\u6392\u884c\u699c<sup class="ost_icon_reddot" id="ost_rank_v"></sup></h3><div class="ost_pop" id="ost_p"></div></li><li class="ost_fr ost_log ost_bg" id="ost_log"></li></ul><div id="ost_d" class="ost_big"></div>',
        e.body.appendChild(t),
        e.body.style.paddingTop = "42px",
        this
    },
    loadO2Media: function () {
      return l.loadJS("//game.qq.com/act/media/20120601457/data.js?ran=" + n, function () {
        window.tencentO2AdCallback1 = function (t) {
          if (t) {
            var e = o("ost_g")
              , n = o("ost_d")
              , a = !1
              , s = unescape(t.res_url_small)
              , i = unescape(t.res_url)
              , l = t.link_to;
            e.innerHTML = '<img class="ost_nb" id="ost_go" src="' + s + '" alt=""/>',
              e.onmouseover = n.onmouseover = function () {
                n.style.display = "block",
                  o("ost_go").style.display = "none",
                  a || (n.innerHTML = '<a rel="noopener" href="' + l + '" target="_blank"><img class="ost_nb" src="' + i + '" width="' + t.width + '" height="' + t.height + '" alt=""/></a>'),
                  a = !0
              }
              ,
              e.onmouseout = n.onmouseout = function () {
                n.style.display = "none",
                  o("ost_go").style.display = "block"
              }
          }
        }
          ,
          l.loadJS("//ac.o2.qq.com/php/show.php?loc_id=119_0d8e2b9df01ce2966bb5d8dd52e865e1&func_type=1&v=1&ran=" + n, "", {
            charset: "utf-8"
          })
      }),
        this
    },
    footMedia: function () {
      return l.loadJS("//game.qq.com/act/media/20120601457/data.js?ran=" + n, function () {
        var t = window.location.href
          , o = _tencent_media.except.split(",")
          , n = e.title
          , a = !1
          , s = !0;
        if (o.length && "\u65e0" != o[0])
          for (var l = o.length; l--;)
            if (n.indexOf(o[l]) != -1) {
              s = !1;
              break
            }
        for (var r = 1, c = _tencent_media.prod.length; r < c; r++) {
          var d = _tencent_media.prod[r].site;
          if (t == d || t == d + "/" || t == d + "/index.shtml" || t.indexOf(d + "?") != -1 || t.indexOf(d + "/?") != -1 || t.indexOf(d + "/index.shtml?") != -1 || t.indexOf(d + "/main.shtml?") != -1 || t.indexOf(d + "#") != -1 || t.indexOf(d + "/#") != -1 || t.indexOf(d + "/main.shtml#") != -1) {
            a = !0;
            break
          }
        }
        if (a && s) {
          var m = e.createElement("div")
            , _ = _tencent_media.ads.main;
          e.body.appendChild(m);
          var u = null
            , h = _[1]
            , f = "?";
          h.indexOf("?") != -1 && (f = "&");
          var p = '<div class="ost_bpb"><h3 class="ost_t ost_bg"><a href="javascript:bps(false);" class="ost_bpc ost_fr ost_bg ost_hdn">\u5173\u95ed</a>\u817e\u8baf\u6e38\u620f\u7cbe\u54c1\u63a8\u8350</h3><p style="background-image:url(' + _[0] + ')" class="ost_p ost_bg"><a href="' + h + f + 'ADTAG=media.free.gamewebhot.ad" rel="noopener" class="ost_lnk ost_hdn" target="_blank">\u70b9\u51fb\u8fdb\u5165</a></p></div>'
            , g = '<a href="javascript:bps(true);" class="ost_cnr ost_bg ost_hdn">\u70b9\u51fb\u8fdb\u5165</a>'
            , v = function (t) {
              if (t ? (m.innerHTML = p,
                u = 174) : (m.innerHTML = g,
                  u = 53),
                b && clearTimeout(b),
                i) {
                var o = function () {
                  m.style.top = e.documentElement.scrollTop + e.documentElement.clientHeight - u + "px"
                };
                o(),
                  window.onscroll = o,
                  window.attachEvent("onresize", o)
              }
            };
          window.bps = v,
            m.className = "ost_bp",
            m.style.cssText = "position:absolute;right:-500px;",
            v(!0);
          var b = setTimeout(function () {
            v(!1),
              b = null,
              clearTimeout(b)
          }, 8e3)
        }
      }),
        this
    },
    tgConsole: function () {
      return window.console && !e.all && console.log("\n%cTGideas\n%c\u6211\u4eec\u7684\u535a\u5ba2\u5730\u5740://tgideas.qq.com?ADTAG=media.gameweb.console\n%c\u6211\u4eec\u7684\u89e3\u51b3\u65b9\u6848://tguide.qq.com?ADTAG=media.gameweb.console", 'font-family:Consolas,Monaco,"Courier New",Helvetica;font-size:30px;color:#000;line-height:25px;', "color:#333;line-height:30px", "color:#333;"),
        this
    },
    rankEffct: function () {
      function t () {
        var t = l.Cookie.get("bRankChanged")
          , e = o("ost_rank_v");
        "TRUE" == t ? e.className = "ost_icon_reddot ost_bg" : e.className = "ost_icon_reddot"
      }
      var e = o("ost_p")
        , a = o("ost_t")
        , s = "//game.gtimg.cn/images/js/title/title_game_rank.html?rd=" + n;
      return l.eventUtil.addListener(a, "mouseenter", function (n) {
        a.className = "ost_title ost_h40",
          !e.innerHTML && (e.innerHTML = '<iframe id="gameRank" name="gameRank" allowTransparency="true" style="background:transparent;" src="' + s + '" width="708" height="582" frameBorder="0" scrolling="no"></iframe></div>'),
          e.style.display = "block";
        var i = o("gameRank");
        i.attachEvent ? i.attachEvent("onload", function () {
          t()
        }) : i.onload = function () {
          t()
        }
          ,
          l.eventUtil.stopPropagation(n)
      }),
        l.eventUtil.addListener(e, "mouseenter", function (t) {
          a.className = "ost_title ost_h40",
            e.style.display = "block",
            l.eventUtil.stopPropagation(t)
        }),
        l.eventUtil.addListener(a, "mouseleave", function (t) {
          e.style.display = "none",
            a.className = "ost_title ost_h40",
            l.Cookie.clear("bRankChanged"),
            l.eventUtil.stopPropagation(t)
        }),
        l.eventUtil.addListener(e, "mouseleave", function (t) {
          e.style.display = "none",
            a.className = "ost_title ost_h40",
            l.Cookie.clear("bRankChanged"),
            l.eventUtil.stopPropagation(t)
        }),
        this
    }
  },
    r.init(),
    "undefined" == typeof ostb_int && (window.ostb_int = function () { }
    )
}(window, window.document);
/*  |xGv00|a97320df9630cb9dc168b762bb1626b3 */