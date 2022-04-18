# public-work
HTML source code
<!DOCTYPE html><html lang="en-US" dir="ltr"><head><meta charset="UTF-8"><meta http-equiv="Cache-Control" content="no-cache"/><meta http-equiv="pragma" content="no-cache"/><title>Google AdMob</title><script>window.$acx = {xsrfToken: 'ALwxsBFjYUb5Thihkse0lkuLWM3yYT96Tg:1649965695984',};</script><script>(function(){/*

 Copyright The Closure Library Authors.
 SPDX-License-Identifier: Apache-2.0
*/
'use strict';var e="function"==typeof Object.defineProperties?Object.defineProperty:function(a,b,c){if(a==Array.prototype||a==Object.prototype)return a;a[b]=c.value;return a};function m(a){a=["object"==typeof globalThis&&globalThis,a,"object"==typeof window&&window,"object"==typeof self&&self,"object"==typeof global&&global];for(var b=0;b<a.length;++b){var c=a[b];if(c&&c.Math==Math)return c}throw Error("Cannot find global object");}var n=m(this);
function q(a,b){if(b)a:{var c=n;a=a.split(".");for(var d=0;d<a.length-1;d++){var f=a[d];if(!(f in c))break a;c=c[f]}a=a[a.length-1];d=c[a];b=b(d);b!=d&&null!=b&&e(c,a,{configurable:!0,writable:!0,value:b})}}var r="function"==typeof Object.assign?Object.assign:function(a,b){for(var c=1;c<arguments.length;c++){var d=arguments[c];if(d)for(var f in d)Object.prototype.hasOwnProperty.call(d,f)&&(a[f]=d[f])}return a};q("Object.assign",function(a){return a||r});var u=this||self;function v(a){return new u.Promise(a)}
function w(a,b){b=void 0===b?{}:b;if("fetch"in u)return u.fetch(a,b);var c=new XMLHttpRequest,d=b.method||"GET",f=b.headers||{},h=b.body;return v(function(l,g){c.addEventListener("readystatechange",function(){4==c.readyState&&(200<=c.status&&300>c.status?l({ok:!0,status:c.status,text:function(){return u.Promise.resolve(c.responseText)}}):g({ok:!1,status:c.status,text:function(){return u.Promise.resolve(c.responseText)}}))});c.open(d,a);for(var k in f)c.setRequestHeader(k,f[k]);c.send(h)})}
function x(a,b){return v(function(c,d){function f(h){a().then(function(l){return c(Object.assign({},{value:l},h))})["catch"](function(l){h.failureTimestamps.push((new Date).getTime());h.retries===b?d(Object.assign({},{exception:l},h)):setTimeout(function(){h.retries+=1;h.attemptTimestamps.push((new Date).getTime());return f(h)},1E3*(Math.pow(2,h.retries)+Math.random()))})}f({retries:0,attemptTimestamps:[(new Date).getTime()],failureTimestamps:[],allowedAttempts:b})})};var y=[],z={},A=0,B;function C(a,b){return y.filter(function(c){return c.startTime>=a&&c.startTime+c.duration<=b})}function D(a){z[a]=performance.now();0>=A&&B.observe({entryTypes:["longtask"]});A=Math.max(0,A+1)}function E(a){var b=performance.now(),c=z[a];delete z[a];A--;"takeRecords"in B&&Array.prototype.push.apply(y,B.takeRecords());a=C(c,b);0>=A&&(B.disconnect(),A=y.length=0);return a};var F={},G={},H,I,J=0;function L(a){a.forEach(function(b){b.name in F&&(F[b.name]={startTime:b.startTime,responseStart:b.responseStart,responseEnd:b.responseEnd,transferSize:b.transferSize})})}function M(a,b){1E3>=J+1&&!(a in G)&&(J++,G[a]=b||a,F[b||a]=!0)}function N(a){var b=G[a],c=F[b];J-=c?1:0;1==c&&(L(I()),c=F[b]);delete F[b];delete G[a];return 1==c?void 0:c}function O(a){var b=G[a],c=F[b];delete F[b];delete G[a];J-=c?1:0};/*

 SPDX-License-Identifier: Apache-2.0
*/
function P(a,b){b={src:a,retryResult:b};"$acx"in u&&"resourceTimingBuffer"in u.$acx&&(b.performanceEntry=u.$acx.resourceTimingBuffer.get(a));return b}function Q(a){return v(function(b,c){try{"function"===typeof a&&a(),b()}catch(d){c(d)}})}function R(a,b){var c={},d;for(d in b)b.hasOwnProperty(d)&&(a.hasOwnProperty(d)?c[d]=a[d]:c[d]=b[d]);return c}function S(){var a=document.createElement("script");"nonce"in a?a.nonce=u.$acx.cspNonce:a.setAttribute("nonce",u.$acx.cspNonce);return a}
function T(a){var b=void 0===b?w:b;u.dart_requestedScripts=u.dart_requestedScripts||[];this.i=this.h=null;this.s=b;this.g={};this.m=a}T.prototype.load=function(a,b){b=void 0===b?{}:b;b=R(b,U);return V(this,a.src,function(){return W(a.cloneNode(!1))},b.retries,b.track,b.dedupe)};
T.prototype.u=function(a,b){b=void 0===b?{}:b;b=R(b,U);var c=b.retries,d=b.track;b=b.dedupe;var f=S();if(!this.m)throw"loadUrlUsingScriptTag API cannot be used without providing a scriptSrcSetter.";this.m(f,a);return this.load(f,{B:c,track:d,A:b})};
T.prototype.v=function(a,b){var c=this;b=void 0===b?{}:b;b=R(b,aa);var d=b.retries,f=b.track,h=b.dedupe,l=b.beforeExecute,g=b.requestPayload,k=b.contentType;if(b.xsrfProtected){var p={method:"POST",headers:{"X-Framework-Xsrf-Token":u.$acx.xsrfToken}};void 0!==g&&""!==g&&(p.body=g,p.headers["Content-Type"]=k)}return V(this,a,function(){var t=p;t=void 0===t?{method:"GET"}:t;return c.s(a,t)},d,f,h,function(t){return t.text().then(function(ba){return Q(l).then(function(){var K=S();K.appendChild(document.createTextNode(ba));
document.head.appendChild(K)})})})};
function V(a,b,c,d,f,h,l){if(h&&b in a.g)return a.g[b];d=c=x(c,d);l&&(d=c.then(function(g){return l(g.value).then(function(){return g}).catch(function(k){g.exception=k;return g})}));b in a.g||(a.g[b]=d);return f?(u.dart_requestedScripts.push(b),"$acx"in u&&"resourceTimingBuffer"in u.$acx&&u.$acx.resourceTimingBuffer.add(b),d.then(function(g){if("acx_Observable"in u){var k=P(b,g);a.l().mutate(function(p){p.push(k)});g.performanceEntry=k.performanceEntry}return g}).catch(function(g){if("acx_Observable"in u){var k=
P(b,g);a.j().mutate(function(p){p.push(k)});g.performanceEntry=k.performanceEntry}return g})):d}function W(a){document.head.appendChild(a);return v(function(b,c){a.onload=b;a.onerror=function(d){a.remove();c(d)}})}T.prototype.l=function(){return this.i=this.i||new u.acx_Observable([])};T.prototype.j=function(){return this.h=this.h||new u.acx_Observable([])};T.prototype.o=function(){this.i=this.h=null};
var U={retries:2,track:!0,dedupe:!1},aa={retries:2,track:!0,dedupe:!1,xsrfProtected:!0,beforeExecute:function(){},requestPayload:void 0,contentType:"application/x-www-form-urlencoded"};var X=u.$acx=u.$acx||{};X.ScriptLoaderFactory={newInstance:function(a){a=new T(a);return{load:a.load.bind(a),loadUrlUsingScriptTag:a.u.bind(a),loadUrlUsingXhr:a.v.bind(a),failedScripts:a.j.bind(a),loadedScripts:a.l.bind(a),defaults:U,reset:a.o.bind(a)}}};(function(a,b){["mousedown","keydown","touchstart"].forEach(function(c){a.addEventListener(c,function(d){b.inputTimeStamp=d.timeStamp},{capture:!0,passive:!0})})})(document.documentElement,X);var Y;
"performance"in u&&"PerformanceObserver"in u?(H=new PerformanceObserver(function(a){return L(a.getEntries())}),H.observe({entryTypes:["resource"]}),"takeRecords"in H?I=H.takeRecords.bind(H):"getEntriesByType"in performance&&(I=function(){var a=performance.getEntriesByType("resource");"clearResourceTimings"in performance&&performance.clearResourceTimings();return a}),Y=!0):Y=!1;
Y&&(X.resourceTimingBuffer={add:M,get:N,remove:O},u._resourceTimingBuffer={add:X.resourceTimingBuffer.add,get:function(a){(a=X.resourceTimingBuffer.get(a))&&(a.fetchStart=a.startTime);return a}});var Z;"PerformanceLongTaskTiming"in u&&"PerformanceObserver"in u&&"performance"in u?(B=new PerformanceObserver(function(a){Array.prototype.push.apply(y,a.getEntries())}),Z=!0):Z=!1;Z&&(X.LongTaskTracker={start:D,stop:E});}).call(this);
</script><script>(function () {function scriptSrcSetter(scriptElement, url){scriptElement.src = url;}window.$acx.scriptLoader = window.$acx.ScriptLoaderFactory.newInstance(scriptSrcSetter);})();</script><style>@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:local('Roboto Regular'),local('Roboto-Regular'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOmCnqEu92Fr1Mu72xKKTU1Kvnz.woff2)format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:local('Roboto Regular'),local('Roboto-Regular'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOmCnqEu92Fr1Mu5mxKKTU1Kvnz.woff2)format('woff2');unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:local('Roboto Regular'),local('Roboto-Regular'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOmCnqEu92Fr1Mu7mxKKTU1Kvnz.woff2)format('woff2');unicode-range:U+1F00-1FFF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:local('Roboto Regular'),local('Roboto-Regular'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOmCnqEu92Fr1Mu4WxKKTU1Kvnz.woff2)format('woff2');unicode-range:U+0370-03FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:local('Roboto Regular'),local('Roboto-Regular'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOmCnqEu92Fr1Mu7WxKKTU1Kvnz.woff2)format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:local('Roboto Regular'),local('Roboto-Regular'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOmCnqEu92Fr1Mu7GxKKTU1Kvnz.woff2)format('woff2');unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:local('Roboto Regular'),local('Roboto-Regular'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOmCnqEu92Fr1Mu4mxKKTU1Kg.woff2)format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:local('Roboto Medium'),local('Roboto-Medium'),local('sans-serif-medium'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmEU9fCRc4AMP6lbBP.woff2)format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:local('Roboto Medium'),local('Roboto-Medium'),local('sans-serif-medium'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmEU9fABc4AMP6lbBP.woff2)format('woff2');unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:local('Roboto Medium'),local('Roboto-Medium'),local('sans-serif-medium'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmEU9fCBc4AMP6lbBP.woff2)format('woff2');unicode-range:U+1F00-1FFF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:local('Roboto Medium'),local('Roboto-Medium'),local('sans-serif-medium'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmEU9fBxc4AMP6lbBP.woff2)format('woff2');unicode-range:U+0370-03FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:local('Roboto Medium'),local('Roboto-Medium'),local('sans-serif-medium'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmEU9fCxc4AMP6lbBP.woff2)format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:local('Roboto Medium'),local('Roboto-Medium'),local('sans-serif-medium'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmEU9fChc4AMP6lbBP.woff2)format('woff2');unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:local('Roboto Medium'),local('Roboto-Medium'),local('sans-serif-medium'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmEU9fBBc4AMP6lQ.woff2)format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD;}@font-face{font-family:'Roboto';font-style:normal;font-weight:700;font-display:swap;src:local('Roboto Bold'),local('Roboto-Bold'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmWUlfCRc4AMP6lbBP.woff2)format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F;}@font-face{font-family:'Roboto';font-style:normal;font-weight:700;font-display:swap;src:local('Roboto Bold'),local('Roboto-Bold'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmWUlfABc4AMP6lbBP.woff2)format('woff2');unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116;}@font-face{font-family:'Roboto';font-style:normal;font-weight:700;font-display:swap;src:local('Roboto Bold'),local('Roboto-Bold'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmWUlfCBc4AMP6lbBP.woff2)format('woff2');unicode-range:U+1F00-1FFF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:700;font-display:swap;src:local('Roboto Bold'),local('Roboto-Bold'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmWUlfBxc4AMP6lbBP.woff2)format('woff2');unicode-range:U+0370-03FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:700;font-display:swap;src:local('Roboto Bold'),local('Roboto-Bold'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmWUlfCxc4AMP6lbBP.woff2)format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB;}@font-face{font-family:'Roboto';font-style:normal;font-weight:700;font-display:swap;src:local('Roboto Bold'),local('Roboto-Bold'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmWUlfChc4AMP6lbBP.woff2)format('woff2');unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:700;font-display:swap;src:local('Roboto Bold'),local('Roboto-Bold'),local('sans-serif'),url(//fonts.gstatic.com/s/roboto/v18/KFOlCnqEu92Fr1MmWUlfBBc4AMP6lQ.woff2)format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD;}</style><style>@font-face{font-family:'Google Sans';font-style:normal;font-weight:400;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2ugCIhM907-0x.woff2)format('woff2');unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:400;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2vQCIhM907-0x.woff2)format('woff2');unicode-range:U+0370-03FF;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:400;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2vACIhM907-0x.woff2)format('woff2');unicode-range:U+0590-05FF,U+200C-2010,U+20AA,U+25CC,U+FB1D-FB4F;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:400;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2sQCIhM907-0x.woff2)format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:400;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2sACIhM907-0x.woff2)format('woff2');unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:400;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2vgCIhM907w.woff2)format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:500;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2ugCIhM907-0x.woff2)format('woff2');unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:500;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2vQCIhM907-0x.woff2)format('woff2');unicode-range:U+0370-03FF;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:500;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2vACIhM907-0x.woff2)format('woff2');unicode-range:U+0590-05FF,U+200C-2010,U+20AA,U+25CC,U+FB1D-FB4F;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:500;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2sQCIhM907-0x.woff2)format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:500;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2sACIhM907-0x.woff2)format('woff2');unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:500;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2vgCIhM907w.woff2)format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:700;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2ugCIhM907-0x.woff2)format('woff2');unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:700;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2vQCIhM907-0x.woff2)format('woff2');unicode-range:U+0370-03FF;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:700;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2vACIhM907-0x.woff2)format('woff2');unicode-range:U+0590-05FF,U+200C-2010,U+20AA,U+25CC,U+FB1D-FB4F;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:700;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2sQCIhM907-0x.woff2)format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:700;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2sACIhM907-0x.woff2)format('woff2');unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF;}@font-face{font-family:'Google Sans';font-style:normal;font-weight:700;font-display:swap;src:url(//fonts.gstatic.com/s/googlesans/v29/4UaRrENHsxJlGDuGo1OIlJfC6mGS6vhAK1YobMu2vgCIhM907w.woff2)format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD;}</style><style>@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:400;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8FacM9Wef3EJPWRrHjgE4B6CnlZxHVDvr9oT3ZQZRENA.woff2)format('woff2');unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:400;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8FacM9Wef3EJPWRrHjgE4B6CnlZxHVDv39oT3ZQZRENA.woff2)format('woff2');unicode-range:U+0370-03FF;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:400;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8FacM9Wef3EJPWRrHjgE4B6CnlZxHVDvH9oT3ZQZRENA.woff2)format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:400;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8FacM9Wef3EJPWRrHjgE4B6CnlZxHVDvD9oT3ZQZRENA.woff2)format('woff2');unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:400;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8FacM9Wef3EJPWRrHjgE4B6CnlZxHVDv79oT3ZQZQ.woff2)format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:500;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8IacM9Wef3EJPWRrHjgE4B6CnlZxHVBg3etBT7TL5-PQEKcA.woff2)format('woff2');unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:500;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8IacM9Wef3EJPWRrHjgE4B6CnlZxHVBg3etBP7TL5-PQEKcA.woff2)format('woff2');unicode-range:U+0370-03FF;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:500;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8IacM9Wef3EJPWRrHjgE4B6CnlZxHVBg3etB_7TL5-PQEKcA.woff2)format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:500;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8IacM9Wef3EJPWRrHjgE4B6CnlZxHVBg3etB77TL5-PQEKcA.woff2)format('woff2');unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:500;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8IacM9Wef3EJPWRrHjgE4B6CnlZxHVBg3etBD7TL5-PQE.woff2)format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:700;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8IacM9Wef3EJPWRrHjgE4B6CnlZxHVBkXYtBT7TL5-PQEKcA.woff2)format('woff2');unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:700;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8IacM9Wef3EJPWRrHjgE4B6CnlZxHVBkXYtBP7TL5-PQEKcA.woff2)format('woff2');unicode-range:U+0370-03FF;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:700;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8IacM9Wef3EJPWRrHjgE4B6CnlZxHVBkXYtB_7TL5-PQEKcA.woff2)format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:700;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8IacM9Wef3EJPWRrHjgE4B6CnlZxHVBkXYtB77TL5-PQEKcA.woff2)format('woff2');unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF;}@font-face{font-family:'Google Sans Display';font-style:normal;font-weight:700;font-display:swap;src:url(//fonts.gstatic.com/s/googlesansdisplay/v14/ea8IacM9Wef3EJPWRrHjgE4B6CnlZxHVBkXYtBD7TL5-PQE.woff2)format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD;}</style><style>@font-face{font-family:'Material Icons Extended';font-style:normal;font-weight:400;src:url(//fonts.gstatic.com/s/materialiconsextended/v109/kJEjBvgX7BgnkSrUwT8UnLVc38YydejYY-oE_LvJHMXBBA.woff2)format('woff2');}.material-icons-extended{font-family:'Material Icons Extended';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased;}</style><style>@font-face{font-family:'Google Material Icons';font-style:normal;font-weight:400;src:url(//fonts.gstatic.com/s/googlematerialicons/v105/Gw6kwdfw6UnXLJCcmafZyFRXb3BL9rvi0QZG3Sy7X00.woff2)format('woff2');}.google-material-icons{font-family:'Google Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased;}</style><link rel="icon" type="image/x-icon" sizes="32x32" href="https://www.google.com/admob/images/admob-favicon.ico"/><style>html, body {height: 100%; margin: 0; padding: 0; width: 100%;}body {font-family: 'Roboto', sans-serif; font-size: 13px; -moz-osx-font-smoothing: grayscale; -webkit-font-smoothing: antialiased; -webkit-overflow-scrolling: touch; -webkit-text-size-adjust: 100%;}ipl-progress-indicator {opacity: 1; pointer-events: none; -webkit-transition: opacity cubic-bezier(.4, 0, .2, 1) 436ms; transition: opacity cubic-bezier(.4, 0, .2, 1) 436ms; z-index: 9999;}ipl-progress-indicator.hide {opacity: 0;}ipl-progress-indicator .first-indicator, ipl-progress-indicator .second-indicator {background-color: #4285f4; bottom: 0; left: 0; right: 0; top: 0; position: absolute; -webkit-transform-origin: left center; transform-origin: left center; -webkit-transform: translate3d(0, 0, 0) scaleX(0); transform: scaleX(0); will-change: transform;}ipl-progress-indicator .first-indicator {-webkit-animation: first-indicator 2000ms linear infinite; animation: first-indicator 2000ms linear infinite;}ipl-progress-indicator .second-indicator {-webkit-animation: second-indicator 2000ms linear infinite; animation: second-indicator 2000ms linear infinite;}ipl-progress-indicator > .admob-logo-frame {display: -webkit-flex; display: flex; -webkit-flex-direction: column; flex-direction: column; -webkit-justify-content: center; justify-content: center; -webkit-animation: fadein 436ms; animation: fadein 436ms; height: 98%;}ipl-progress-indicator .admob-logo {-webkit-align-self: center; align-self: center;}@-webkit-keyframes fadein {from { opacity: 0; }to   { opacity: 1; }}@keyframes fadein {from { opacity: 0; }to   { opacity: 1; }}@-webkit-keyframes first-indicator {0% {-webkit-transform: translate3d(0%, 0, 0) scaleX(0);}25% {-webkit-transform: translate3d(0%, 0, 0) scaleX(0.5);}50% {-webkit-transform: translate3d(25%, 0, 0) scaleX(0.75);}75% {-webkit-transform: translate3d(100%, 0, 0) scaleX(0);}100% {-webkit-transform: translate3d(100%, 0, 0) scaleX(0);}}@keyframes first-indicator {0% {transform: translateX(0vw) scaleX(0);}25% {transform: translateX(0vw) scaleX(0.5);}50% {transform: translateX(25vw) scaleX(0.75);}75% {transform: translateX(100vw) scaleX(0);}100% {transform: translateX(100vw) scaleX(0);}}@-webkit-keyframes second-indicator {0% {-webkit-transform: translate3d(0%, 0, 0) scaleX(0);}60% {-webkit-transform: translate3d(0%, 0, 0) scaleX(0);}80% {-webkit-transform: translate3d(0%, 0, 0) scaleX(0.6);}100% {-webkit-transform: translate3d(100%, 0, 0) scaleX(0.1);}}@keyframes second-indicator {0% {transform: translateX(0vw) scaleX(0);}60% {transform: translateX(0vw) scaleX(0);}80% {transform: translateX(0vw) scaleX(0.6);}100% {transform: translateX(100vw) scaleX(0.1);}}</style><script>
      window['GoogleAnalyticsObject']='gaController';window.gaController=window.gaController||function(){(gaController.q=gaController.q||[]).push(arguments)};gaController.l=+new Date;
    gaController('create', 'UA-86618834-1', 'auto', 'admobTracker'); gaController('admobTracker.send', 'pageview');</script><script async src='//www.google-analytics.com/analytics.js'></script><meta name="viewport" content="width=device-width, initial-scale=1"><script type="text/javascript">window.eventCallbacks=window.eventCallbacks||[];window.registerEventCallback=window.registerEventCallback||function(f){var i=0;for(var length=window.eventCallbacks.length;i<length;i++){var cb=window.eventCallbacks[i];if(!cb)break}window.eventCallbacks[i]=f;return i};window.unregisterEventCallback=window.unregisterEventCallback||function(i){window.eventCallbacks[i]=null};
window.sendEvent=window.sendEvent||function(){for(var i=0,length=window.eventCallbacks.length;i<length;i++){var cb=window.eventCallbacks[i];try{if(cb)cb.apply(null,arguments)}catch(e){window.unregisterEventCallback(i);if(window.console){var func=window.console.error||window.console.info||window.console.log;if(func)func.call(window.console,"An error occured while processing callback: "+e)}}}};
</script><script type='text/javascript'>var sessionId= 3.6660405818381921E18 ;</script></head><body><ipl-progress-indicator style="background-color: #f8f9fa; width: 100%; height: 100%; position:fixed;" class="hide"><div style="background-color: #c6dafc; height: 4px; overflow: hidden; position: relative;"><div class="first-indicator"></div><div class="second-indicator"></div></div><div class="admob-logo-frame"><svg xmlns="http://www.w3.org/2000/svg" width="112" height="112" viewBox="0 0 192 192" class="admob-logo"><path fill="none" d="M0 0h192v192H0z"/><path fill="#FBBC04" d="M92.01 8.26c1.27-.26 6.3-.25 7.5-.26 34.25-.27 81.75 28.87 84.49 84.28v69.18c0 12.45-10.28 22.54-22.77 22.54-9 0-21.23-11.53-21.23-22.5V92.32c-1.27-18.26-16.07-38.81-40.99-40.36-1.54-.1-5.04-.16-7.01.1"/><path fill="#4285F4" d="M183.98 162c0 12.15-9.85 22-22 22S140 174.15 140 162s9.83-22 21.98-22 22 9.85 22 22z"/><path fill="#EA4335" d="M93.2 183.24c12.6 0 22.81-10.02 22.81-22.37 0-12.36-10.46-21.33-23.05-21.33-.08 0-.16.01-.24.01-21.66-1.5-41.92-20.57-40.44-46.71 0 0 .01-.13.03-.42 1.25-20.51 18.75-39.12 40.9-40.4 12.6 0 22.81-9.04 22.81-21.39S105.8 8.25 93.2 8.25c-.51 0-1.02-.03-1.53 0C53.46 9.58 8.46 41.37 8.01 95.4v.33c0 54.83 48.09 87.5 83.93 87.5h1.26z"/></svg></div></ipl-progress-indicator><script>
    (function() {
      var progressIndicator = document.querySelector('ipl-progress-indicator');
      var ow = progressIndicator.offsetWidth;
      requestAnimationFrame(function() {
        progressIndicator.className = '';
      });
    })();
    </script><div id="adblock" style="height: 1px; position: absolute;"></div><script>(function() {var callbacks = []; window.onAdBlockerDetected
