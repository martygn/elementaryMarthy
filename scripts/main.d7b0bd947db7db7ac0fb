/*! For license information please see main.d7b0bd947db7db7ac0fb.js.LICENSE.txt */
(self.webpackChunkmvp = self.webpackChunkmvp || []).push([[792], {
    491: function(t, n, e) {
        var o, i, r;
        r = function() {
            var t, n, e = document, o = e.getElementsByTagName("head")[0], i = "push", r = "readyState", a = "onreadystatechange", c = {}, u = {}, s = {}, l = {};
            function f(t, n) {
                for (var e = 0, o = t.length; e < o; ++e)
                    if (!n(t[e]))
                        return !1;
                return 1
            }
            function h(t, n) {
                f(t, (function(t) {
                    return n(t),
                    1
                }
                ))
            }
            function d(n, e, o) {
                n = n[i] ? n : [n];
                var r = e && e.call
                  , a = r ? e : o
                  , v = r ? n.join("") : e
                  , m = n.length;
                function g(t) {
                    return t.call ? t() : c[t]
                }
                function w() {
                    if (!--m)
                        for (var t in c[v] = 1,
                        a && a(),
                        s)
                            f(t.split("|"), g) && !h(s[t], g) && (s[t] = [])
                }
                return setTimeout((function() {
                    h(n, (function n(e, o) {
                        return null === e ? w() : (o || /^https?:\/\//.test(e) || !t || (e = -1 === e.indexOf(".js") ? t + e + ".js" : t + e),
                        l[e] ? (v && (u[v] = 1),
                        2 == l[e] ? w() : setTimeout((function() {
                            n(e, !0)
                        }
                        ), 0)) : (l[e] = 1,
                        v && (u[v] = 1),
                        void p(e, w)))
                    }
                    ))
                }
                ), 0),
                d
            }
            function p(t, i) {
                var c, u = e.createElement("script");
                u.onload = u.onerror = u[a] = function() {
                    u[r] && !/^c|loade/.test(u[r]) || c || (u.onload = u[a] = null,
                    c = 1,
                    l[t] = 2,
                    i())
                }
                ,
                u.async = 1,
                u.src = n ? t + (-1 === t.indexOf("?") ? "?" : "&") + n : t,
                o.insertBefore(u, o.lastChild)
            }
            return d.get = p,
            d.order = function(t, n, e) {
                !function o(i) {
                    i = t.shift(),
                    t.length ? d(i, o) : d(i, n, e)
                }()
            }
            ,
            d.path = function(n) {
                t = n
            }
            ,
            d.urlArgs = function(t) {
                n = t
            }
            ,
            d.ready = function(t, n, e) {
                t = t[i] ? t : [t];
                var o, r = [];
                return !h(t, (function(t) {
                    c[t] || r[i](t)
                }
                )) && f(t, (function(t) {
                    return c[t]
                }
                )) ? n() : (o = t.join("|"),
                s[o] = s[o] || [],
                s[o][i](n),
                e && e(r)),
                d
            }
            ,
            d.done = function(t) {
                d([null], t)
            }
            ,
            d
        }
        ,
        t.exports ? t.exports = r() : void 0 === (i = "function" == typeof (o = r) ? o.call(n, e, n, t) : o) || (t.exports = i)
    },
    713: function(t, n, e) {
        "use strict";
        var o = e(491);
        n.A = new Promise(( (t, n) => {
            o("https://cdn.jsdelivr.net/gh/jquery/jquery@3/dist/jquery.min.js", ( () => (console.log("jQuery loaded"),
            t(window.jQuery))))
        }
        ))
    },
    916: function(t, n, e) {
        "use strict";
        var o = e(713);
        o.A.then((t => {
            t((function() {
                t("a").not('[href*="mailto:"], [href*="magnet:"]').each((function() {
                    -1 === this.href.indexOf(window.location.host) && t(this).attr("target", "_blank").attr("rel", "noopener")
                }
                ))
            }
            ))
        }
        )),
        o.A.then((t => {
            t((function() {
                const n = t(document);
                n.on("click", ".popover > a", (function(e) {
                    e.preventDefault();
                    const o = t("body")
                      , i = t(e.target).parent()
                      , r = i.find(".popover-content");
                    o.css({
                        overflow: "hidden"
                    }),
                    i.addClass("active"),
                    r.on("scroll touchmove mousewheel wheel", (function(t) {
                        t.stopPropagation()
                    }
                    ));
                    const a = i.outerWidth() / 2 - r.outerWidth() / 2;
                    r.css({
                        left: a
                    }),
                    n.one("click scroll touchmove mousewheel wheel", (function(n) {
                        t(n.target).is(".popover-content *") || (n.stopImmediatePropagation(),
                        n.preventDefault()),
                        o.css({
                            overflow: "visible"
                        }),
                        i.removeClass("active"),
                        o.click()
                    }
                    ))
                }
                ))
            }
            ))
        }
        )),
        o.A.then((t => {
            t((function() {
                t(document).on("click", "a", (function(n) {
                    if (n.isDefaultPrevented())
                        return;
                    let e, o = t(this).attr("href");
                    if (null != o && !1 !== o && -1 !== o.indexOf("#") && (o = o.split("#").pop(),
                    "!" !== o[0])) {
                        if ("" === o)
                            e = 0;
                        else {
                            const n = t("#" + o);
                            if (!n.length)
                                return;
                            e = n.offset().top
                        }
                        t("html, body").stop().animate({
                            scrollTop: e
                        }, "normal", (function() {
                            window.location.hash = o
                        }
                        )),
                        n.preventDefault()
                    }
                }
                )),
                setTimeout((function() {
                    t('a[href^="#"]').each((function() {
                        if (!t(this).hasClass("open-modal")) {
                            const n = t(this).attr("href");
                            t(this).attr("href", window.location.pathname + n)
                        }
                    }
                    ))
                }
                ), 0)
            }
            ))
        }
        )),
        o.A.then((t => {
            const n = t("nav .menu-button");
            n.addClass("enabled"),
            n.on("click", (function(t) {
                "true" === n.attr("aria-expanded") ? n.attr("aria-expanded", "false") : n.attr("aria-expanded", "true")
            }
            ))
        }
        ))
    }
}, function(t) {
    t(t.s = 916)
}
]);
//# sourceMappingURL=main.d7b0bd947db7db7ac0fb.js.map
