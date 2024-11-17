<!-- Created by Aplus -->

<!DOCTYPE html>
<html lang="en">

<head><!-- Global site tag (gtag.js) - Google Analytics -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=UA-58936387-12"></script>
    <script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());

    gtag('config', 'UA-58936387-12');
    </script>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
<script>
  // Save the current console log function in case we need it.
  const _log = console.log;
  const _debug = console.debug;
  const _info = console.info;
  const _warn = console.warn;
  const _error = console.error;
  // Override the console
  console.log = function(...rest) {
    window.parent.postMessage(
      {
        source: 'iframe-' + window.name,
        message: rest,
        method: 'log'
      },
      '*'
    );
    _log.apply(console, arguments);
  };

  console.debug = function(...rest) {
    window.parent.postMessage(
      {
        source: 'iframe-' + window.name,
        message: rest,
        method: 'debug'
      },
      '*'
    );
    _debug.apply(console, arguments);
  };

  console.info = function(...rest) {
    window.parent.postMessage(
      {
        source: 'iframe-' + window.name,
        message: rest,
        method: 'info'
      },
      '*'
    );
    _info.apply(console, arguments);
  };

  console.warn = function(...rest) {
    window.parent.postMessage(
      {
        source: 'iframe-' + window.name,
        message: rest,
        method: 'warn'
      },
      '*'
    );
    _warn.apply(console, arguments);
  };

  console.error = function(...rest) {
    window.parent.postMessage(
      {
        source: 'iframe-' + window.name,
        message: rest,
        method: 'error'
      },
      '*'
    );
    _error.apply(console, arguments);
  };
</script>

    
<script>
    window.onerror = function(msg) {
        window.parent.postMessage(
            {
                source: 'iframe-' + window.name,
                message: [msg],
                method: 'error'
            },
            '*'
            );
    };
</script>

    
<script>
    window.addEventListener('load', (event) => {
    window.parent.postMessage({
        source: 'iframe-navigation-' + window.name,
        message: document.location.href,
    }, '*');
    })
</script>

    
<script>
    window.onload = function() {
        window.parent.postMessage(
            {
              source: 'iframe-' + window.name,
              windowHeight: document.getElementsByTagName('html')[0].getBoundingClientRect().height,
            },
            '*'
          );
    };
</script>

          <meta charset="utf-8"><script type="text/javascript">(window.NREUM||(NREUM={})).init={ajax:{deny_list:["bam.nr-data.net"]}};(window.NREUM||(NREUM={})).loader_config={licenseKey:"1e7946724e",applicationID:"31671751"};;/*! For license information please see nr-loader-rum-1.270.3.min.js.LICENSE.txt */
(()=>{var e,t,r={8122:(e,t,r)=>{"use strict";r.d(t,{a:()=>i});var n=r(944);function i(e,t){try{if(!e||"object"!=typeof e)return(0,n.R)(3);if(!t||"object"!=typeof t)return(0,n.R)(4);const r=Object.create(Object.getPrototypeOf(t),Object.getOwnPropertyDescriptors(t)),o=0===Object.keys(r).length?e:r;for(let a in o)if(void 0!==e[a])try{if(null===e[a]){r[a]=null;continue}Array.isArray(e[a])&&Array.isArray(t[a])?r[a]=Array.from(new Set([...e[a],...t[a]])):"object"==typeof e[a]&&"object"==typeof t[a]?r[a]=i(e[a],t[a]):r[a]=e[a]}catch(e){(0,n.R)(1,e)}return r}catch(e){(0,n.R)(2,e)}}},2555:(e,t,r)=>{"use strict";r.d(t,{Vp:()=>c,fn:()=>s,x1:()=>u});var n=r(384),i=r(8122);const o={beacon:n.NT.beacon,errorBeacon:n.NT.errorBeacon,licenseKey:void 0,applicationID:void 0,sa:void 0,queueTime:void 0,applicationTime:void 0,ttGuid:void 0,user:void 0,account:void 0,product:void 0,extra:void 0,jsAttributes:{},userAttributes:void 0,atts:void 0,transactionName:void 0,tNamePlain:void 0},a={};function s(e){try{const t=c(e);return!!t.licenseKey&&!!t.errorBeacon&&!!t.applicationID}catch(e){return!1}}function c(e){if(!e)throw new Error("All info objects require an agent identifier!");if(!a[e])throw new Error("Info for ".concat(e," was never set"));return a[e]}function u(e,t){if(!e)throw new Error("All info objects require an agent identifier!");a[e]=(0,i.a)(t,o);const r=(0,n.nY)(e);r&&(r.info=a[e])}},9417:(e,t,r)=>{"use strict";r.d(t,{D0:()=>g,gD:()=>h,xN:()=>p});var n=r(993);const i=e=>{if(!e||"string"!=typeof e)return!1;try{document.createDocumentFragment().querySelector(e)}catch{return!1}return!0};var o=r(2614),a=r(944),s=r(384),c=r(8122);const u="[data-nr-mask]",d=()=>{const e={mask_selector:"*",block_selector:"[data-nr-block]",mask_input_options:{color:!1,date:!1,"datetime-local":!1,email:!1,month:!1,number:!1,range:!1,search:!1,tel:!1,text:!1,time:!1,url:!1,week:!1,textarea:!1,select:!1,password:!0}};return{ajax:{deny_list:void 0,block_internal:!0,enabled:!0,harvestTimeSeconds:10,autoStart:!0},distributed_tracing:{enabled:void 0,exclude_newrelic_header:void 0,cors_use_newrelic_header:void 0,cors_use_tracecontext_headers:void 0,allowed_origins:void 0},feature_flags:[],generic_events:{enabled:!0,harvestTimeSeconds:30,autoStart:!0},harvest:{tooManyRequestsDelay:60},jserrors:{enabled:!0,harvestTimeSeconds:10,autoStart:!0},logging:{enabled:!0,harvestTimeSeconds:10,autoStart:!0,level:n.p_.INFO},metrics:{enabled:!0,autoStart:!0},obfuscate:void 0,page_action:{enabled:!0},user_actions:{enabled:!0},page_view_event:{enabled:!0,autoStart:!0},page_view_timing:{enabled:!0,harvestTimeSeconds:30,autoStart:!0},privacy:{cookies_enabled:!0},proxy:{assets:void 0,beacon:void 0},session:{expiresMs:o.wk,inactiveMs:o.BB},session_replay:{autoStart:!0,enabled:!1,harvestTimeSeconds:60,preload:!1,sampling_rate:10,error_sampling_rate:100,collect_fonts:!1,inline_images:!1,fix_stylesheets:!0,mask_all_inputs:!0,get mask_text_selector(){return e.mask_selector},set mask_text_selector(t){i(t)?e.mask_selector="".concat(t,",").concat(u):""===t||null===t?e.mask_selector=u:(0,a.R)(5,t)},get block_class(){return"nr-block"},get ignore_class(){return"nr-ignore"},get mask_text_class(){return"nr-mask"},get block_selector(){return e.block_selector},set block_selector(t){i(t)?e.block_selector+=",".concat(t):""!==t&&(0,a.R)(6,t)},get mask_input_options(){return e.mask_input_options},set mask_input_options(t){t&&"object"==typeof t?e.mask_input_options={...t,password:!0}:(0,a.R)(7,t)}},session_trace:{enabled:!0,harvestTimeSeconds:10,autoStart:!0},soft_navigations:{enabled:!0,harvestTimeSeconds:10,autoStart:!0},spa:{enabled:!0,harvestTimeSeconds:10,autoStart:!0},ssl:void 0}},l={},f="All configuration objects require an agent identifier!";function g(e){if(!e)throw new Error(f);if(!l[e])throw new Error("Configuration for ".concat(e," was never set"));return l[e]}function p(e,t){if(!e)throw new Error(f);l[e]=(0,c.a)(t,d());const r=(0,s.nY)(e);r&&(r.init=l[e])}function h(e,t){if(!e)throw new Error(f);var r=g(e);if(r){for(var n=t.split("."),i=0;i<n.length-1;i++)if("object"!=typeof(r=r[n[i]]))return;r=r[n[n.length-1]]}return r}},3371:(e,t,r)=>{"use strict";r.d(t,{V:()=>f,f:()=>l});var n=r(8122),i=r(384),o=r(6154),a=r(9324);let s=0;const c={buildEnv:a.F3,distMethod:a.Xs,version:a.xv,originTime:o.WN},u={customTransaction:void 0,disabled:!1,isolatedBacklog:!1,loaderType:void 0,maxBytes:3e4,onerror:void 0,ptid:void 0,releaseIds:{},appMetadata:{},session:void 0,denyList:void 0,timeKeeper:void 0,obfuscator:void 0},d={};function l(e){if(!e)throw new Error("All runtime objects require an agent identifier!");if(!d[e])throw new Error("Runtime for ".concat(e," was never set"));return d[e]}function f(e,t){if(!e)throw new Error("All runtime objects require an agent identifier!");d[e]={...(0,n.a)(t,u),...c},Object.hasOwnProperty.call(d[e],"harvestCount")||Object.defineProperty(d[e],"harvestCount",{get:()=>++s});const r=(0,i.nY)(e);r&&(r.runtime=d[e])}},9324:(e,t,r)=>{"use strict";r.d(t,{F3:()=>i,Xs:()=>o,xv:()=>n});const n="1.270.3",i="PROD",o="CDN"},6154:(e,t,r)=>{"use strict";r.d(t,{OF:()=>c,RI:()=>i,WN:()=>d,bv:()=>o,gm:()=>a,mw:()=>s,sb:()=>u});var n=r(1863);const i="undefined"!=typeof window&&!!window.document,o="undefined"!=typeof WorkerGlobalScope&&("undefined"!=typeof self&&self instanceof WorkerGlobalScope&&self.navigator instanceof WorkerNavigator||"undefined"!=typeof globalThis&&globalThis instanceof WorkerGlobalScope&&globalThis.navigator instanceof WorkerNavigator),a=i?window:"undefined"!=typeof WorkerGlobalScope&&("undefined"!=typeof self&&self instanceof WorkerGlobalScope&&self||"undefined"!=typeof globalThis&&globalThis instanceof WorkerGlobalScope&&globalThis),s=Boolean("hidden"===a?.document?.visibilityState),c=/iPad|iPhone|iPod/.test(a.navigator?.userAgent),u=c&&"undefined"==typeof SharedWorker,d=((()=>{const e=a.navigator?.userAgent?.match(/Firefox[/\s](\d+\.\d+)/);Array.isArray(e)&&e.length>=2&&e[1]})(),Date.now()-(0,n.t)())},1687:(e,t,r)=>{"use strict";r.d(t,{Ak:()=>c,Ze:()=>l,x3:()=>u});var n=r(7836),i=r(3606),o=r(860),a=r(2646);const s={};function c(e,t){const r={staged:!1,priority:o.P[t]||0};d(e),s[e].get(t)||s[e].set(t,r)}function u(e,t){e&&s[e]&&(s[e].get(t)&&s[e].delete(t),g(e,t,!1),s[e].size&&f(e))}function d(e){if(!e)throw new Error("agentIdentifier required");s[e]||(s[e]=new Map)}function l(e="",t="feature",r=!1){if(d(e),!e||!s[e].get(t)||r)return g(e,t);s[e].get(t).staged=!0,f(e)}function f(e){const t=Array.from(s[e]);t.every((([e,t])=>t.staged))&&(t.sort(((e,t)=>e[1].priority-t[1].priority)),t.forEach((([t])=>{s[e].delete(t),g(e,t)})))}function g(e,t,r=!0){const o=e?n.ee.get(e):n.ee,s=i.i.handlers;if(!o.aborted&&o.backlog&&s){if(r){const e=o.backlog[t],r=s[t];if(r){for(let t=0;e&&t<e.length;++t)p(e[t],r);Object.entries(r).forEach((([e,t])=>{Object.values(t||{}).forEach((t=>{t[0]?.on&&t[0]?.context()instanceof a.y&&t[0].on(e,t[1])}))}))}}o.isolatedBacklog||delete s[t],o.backlog[t]=null,o.emit("drain-"+t,[])}}function p(e,t){var r=e[1];Object.values(t[r]||{}).forEach((t=>{var r=e[0];if(t[0]===r){var n=t[1],i=e[3],o=e[2];n.apply(i,o)}}))}},7836:(e,t,r)=>{"use strict";r.d(t,{P:()=>c,ee:()=>u});var n=r(384),i=r(8990),o=r(3371),a=r(2646),s=r(5607);const c="nr@context:".concat(s.W),u=function e(t,r){var n={},s={},d={},l=!1;try{l=16===r.length&&(0,o.f)(r).isolatedBacklog}catch(e){}var f={on:p,addEventListener:p,removeEventListener:function(e,t){var r=n[e];if(!r)return;for(var i=0;i<r.length;i++)r[i]===t&&r.splice(i,1)},emit:function(e,r,n,i,o){!1!==o&&(o=!0);if(u.aborted&&!i)return;t&&o&&t.emit(e,r,n);for(var a=g(n),c=h(e),d=c.length,l=0;l<d;l++)c[l].apply(a,r);var p=m()[s[e]];p&&p.push([f,e,r,a]);return a},get:v,listeners:h,context:g,buffer:function(e,t){const r=m();if(t=t||"feature",f.aborted)return;Object.entries(e||{}).forEach((([e,n])=>{s[n]=t,t in r||(r[t]=[])}))},abort:function(){f._aborted=!0,Object.keys(f.backlog).forEach((e=>{delete f.backlog[e]}))},isBuffering:function(e){return!!m()[s[e]]},debugId:r,backlog:l?{}:t&&"object"==typeof t.backlog?t.backlog:{},isolatedBacklog:l};return Object.defineProperty(f,"aborted",{get:()=>{let e=f._aborted||!1;return e||(t&&(e=t.aborted),e)}}),f;function g(e){return e&&e instanceof a.y?e:e?(0,i.I)(e,c,(()=>new a.y(c))):new a.y(c)}function p(e,t){n[e]=h(e).concat(t)}function h(e){return n[e]||[]}function v(t){return d[t]=d[t]||e(f,t)}function m(){return f.backlog}}(void 0,"globalEE"),d=(0,n.Zm)();d.ee||(d.ee=u)},2646:(e,t,r)=>{"use strict";r.d(t,{y:()=>n});class n{constructor(e){this.contextId=e}}},9908:(e,t,r)=>{"use strict";r.d(t,{d:()=>n,p:()=>i});var n=r(7836).ee.get("handle");function i(e,t,r,i,o){o?(o.buffer([e],i),o.emit(e,t,r)):(n.buffer([e],i),n.emit(e,t,r))}},3606:(e,t,r)=>{"use strict";r.d(t,{i:()=>o});var n=r(9908);o.on=a;var i=o.handlers={};function o(e,t,r,o){a(o||n.d,i,e,t,r)}function a(e,t,r,i,o){o||(o="feature"),e||(e=n.d);var a=t[o]=t[o]||{};(a[r]=a[r]||[]).push([e,i])}},3878:(e,t,r)=>{"use strict";function n(e,t){return{capture:e,passive:!1,signal:t}}function i(e,t,r=!1,i){window.addEventListener(e,t,n(r,i))}function o(e,t,r=!1,i){document.addEventListener(e,t,n(r,i))}r.d(t,{DD:()=>o,jT:()=>n,sp:()=>i})},5607:(e,t,r)=>{"use strict";r.d(t,{W:()=>n});const n=(0,r(9566).bz)()},9566:(e,t,r)=>{"use strict";r.d(t,{LA:()=>s,bz:()=>a});var n=r(6154);const i="xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx";function o(e,t){return e?15&e[t]:16*Math.random()|0}function a(){const e=n.gm?.crypto||n.gm?.msCrypto;let t,r=0;return e&&e.getRandomValues&&(t=e.getRandomValues(new Uint8Array(30))),i.split("").map((e=>"x"===e?o(t,r++).toString(16):"y"===e?(3&o()|8).toString(16):e)).join("")}function s(e){const t=n.gm?.crypto||n.gm?.msCrypto;let r,i=0;t&&t.getRandomValues&&(r=t.getRandomValues(new Uint8Array(e)));const a=[];for(var s=0;s<e;s++)a.push(o(r,i++).toString(16));return a.join("")}},2614:(e,t,r)=>{"use strict";r.d(t,{BB:()=>a,H3:()=>n,g:()=>u,iL:()=>c,tS:()=>s,uh:()=>i,wk:()=>o});const n="NRBA",i="SESSION",o=144e5,a=18e5,s={STARTED:"session-started",PAUSE:"session-pause",RESET:"session-reset",RESUME:"session-resume",UPDATE:"session-update"},c={SAME_TAB:"same-tab",CROSS_TAB:"cross-tab"},u={OFF:0,FULL:1,ERROR:2}},1863:(e,t,r)=>{"use strict";function n(){return Math.floor(performance.now())}r.d(t,{t:()=>n})},944:(e,t,r)=>{"use strict";function n(e,t){"function"==typeof console.debug&&console.debug("New Relic Warning: https://github.com/newrelic/newrelic-browser-agent/blob/main/docs/warning-codes.md#".concat(e),t)}r.d(t,{R:()=>n})},5284:(e,t,r)=>{"use strict";r.d(t,{t:()=>c,B:()=>s});var n=r(7836),i=r(6154);const o="newrelic";const a=new Set,s={};function c(e,t){const r=n.ee.get(t);s[t]??={},e&&"object"==typeof e&&(a.has(t)||(r.emit("rumresp",[e]),s[t]=e,a.add(t),function(e={}){try{i.gm.dispatchEvent(new CustomEvent(o,{detail:e}))}catch(e){}}({loaded:!0})))}},8990:(e,t,r)=>{"use strict";r.d(t,{I:()=>i});var n=Object.prototype.hasOwnProperty;function i(e,t,r){if(n.call(e,t))return e[t];var i=r();if(Object.defineProperty&&Object.keys)try{return Object.defineProperty(e,t,{value:i,writable:!0,enumerable:!1}),i}catch(e){}return e[t]=i,i}},6389:(e,t,r)=>{"use strict";function n(e,t=500,r={}){const n=r?.leading||!1;let i;return(...r)=>{n&&void 0===i&&(e.apply(this,r),i=setTimeout((()=>{i=clearTimeout(i)}),t)),n||(clearTimeout(i),i=setTimeout((()=>{e.apply(this,r)}),t))}}function i(e){let t=!1;return(...r)=>{t||(t=!0,e.apply(this,r))}}r.d(t,{J:()=>i,s:()=>n})},5289:(e,t,r)=>{"use strict";r.d(t,{GG:()=>o,sB:()=>a});var n=r(3878);function i(){return"undefined"==typeof document||"complete"===document.readyState}function o(e,t){if(i())return e();(0,n.sp)("load",e,t)}function a(e){if(i())return e();(0,n.DD)("DOMContentLoaded",e)}},384:(e,t,r)=>{"use strict";r.d(t,{NT:()=>o,US:()=>d,Zm:()=>a,bQ:()=>c,dV:()=>s,nY:()=>u,pV:()=>l});var n=r(6154),i=r(1863);const o={beacon:"bam.nr-data.net",errorBeacon:"bam.nr-data.net"};function a(){return n.gm.NREUM||(n.gm.NREUM={}),void 0===n.gm.newrelic&&(n.gm.newrelic=n.gm.NREUM),n.gm.NREUM}function s(){let e=a();return e.o||(e.o={ST:n.gm.setTimeout,SI:n.gm.setImmediate,CT:n.gm.clearTimeout,XHR:n.gm.XMLHttpRequest,REQ:n.gm.Request,EV:n.gm.Event,PR:n.gm.Promise,MO:n.gm.MutationObserver,FETCH:n.gm.fetch,WS:n.gm.WebSocket}),e}function c(e,t){let r=a();r.initializedAgents??={},t.initializedAt={ms:(0,i.t)(),date:new Date},r.initializedAgents[e]=t}function u(e){let t=a();return t.initializedAgents?.[e]}function d(e,t){a()[e]=t}function l(){return function(){let e=a();const t=e.info||{};e.info={beacon:o.beacon,errorBeacon:o.errorBeacon,...t}}(),function(){let e=a();const t=e.init||{};e.init={...t}}(),s(),function(){let e=a();const t=e.loader_config||{};e.loader_config={...t}}(),a()}},2843:(e,t,r)=>{"use strict";r.d(t,{u:()=>i});var n=r(3878);function i(e,t=!1,r,i){(0,n.DD)("visibilitychange",(function(){if(t)return void("hidden"===document.visibilityState&&e());e(document.visibilityState)}),r,i)}},3434:(e,t,r)=>{"use strict";r.d(t,{YM:()=>c});var n=r(7836),i=r(5607);const o="nr@original:".concat(i.W);var a=Object.prototype.hasOwnProperty,s=!1;function c(e,t){return e||(e=n.ee),r.inPlace=function(e,t,n,i,o){n||(n="");const a="-"===n.charAt(0);for(let s=0;s<t.length;s++){const c=t[s],u=e[c];d(u)||(e[c]=r(u,a?c+n:n,i,c,o))}},r.flag=o,r;function r(t,r,n,s,c){return d(t)?t:(r||(r=""),nrWrapper[o]=t,function(e,t,r){if(Object.defineProperty&&Object.keys)try{return Object.keys(e).forEach((function(r){Object.defineProperty(t,r,{get:function(){return e[r]},set:function(t){return e[r]=t,t}})})),t}catch(e){u([e],r)}for(var n in e)a.call(e,n)&&(t[n]=e[n])}(t,nrWrapper,e),nrWrapper);function nrWrapper(){var o,a,d,l;try{a=this,o=[...arguments],d="function"==typeof n?n(o,a):n||{}}catch(t){u([t,"",[o,a,s],d],e)}i(r+"start",[o,a,s],d,c);try{return l=t.apply(a,o)}catch(e){throw i(r+"err",[o,a,e],d,c),e}finally{i(r+"end",[o,a,l],d,c)}}}function i(r,n,i,o){if(!s||t){var a=s;s=!0;try{e.emit(r,n,i,t,o)}catch(t){u([t,r,n,i],e)}s=a}}}function u(e,t){t||(t=n.ee);try{t.emit("internal-error",e)}catch(e){}}function d(e){return!(e&&"function"==typeof e&&e.apply&&!e[o])}},993:(e,t,r)=>{"use strict";r.d(t,{ET:()=>o,p_:()=>i});var n=r(860);const i={ERROR:"ERROR",WARN:"WARN",INFO:"INFO",DEBUG:"DEBUG",TRACE:"TRACE"},o="log";n.K.logging},3969:(e,t,r)=>{"use strict";r.d(t,{TZ:()=>n,XG:()=>s,rs:()=>i,xV:()=>a,z_:()=>o});const n=r(860).K.metrics,i="sm",o="cm",a="storeSupportabilityMetrics",s="storeEventMetrics"},6630:(e,t,r)=>{"use strict";r.d(t,{T:()=>n});const n=r(860).K.pageViewEvent},782:(e,t,r)=>{"use strict";r.d(t,{T:()=>n});const n=r(860).K.pageViewTiming},6344:(e,t,r)=>{"use strict";r.d(t,{G4:()=>i});var n=r(2614);r(860).K.sessionReplay;const i={RECORD:"recordReplay",PAUSE:"pauseReplay",REPLAY_RUNNING:"replayRunning",ERROR_DURING_REPLAY:"errorDuringReplay"};n.g.ERROR,n.g.FULL,n.g.OFF},4234:(e,t,r)=>{"use strict";r.d(t,{W:()=>o});var n=r(7836),i=r(1687);class o{constructor(e,t){this.agentIdentifier=e,this.ee=n.ee.get(e),this.featureName=t,this.blocked=!1}deregisterDrain(){(0,i.x3)(this.agentIdentifier,this.featureName)}}},7603:(e,t,r)=>{"use strict";r.d(t,{j:()=>P});var n=r(860),i=r(2555),o=r(3371),a=r(9908),s=r(7836),c=r(1687),u=r(5289),d=r(6154),l=r(944),f=r(3969),g=r(384),p=r(6344);const h=["setErrorHandler","finished","addToTrace","addRelease","addPageAction","setCurrentRouteName","setPageViewName","setCustomAttribute","interaction","noticeError","setUserId","setApplicationVersion","start",p.G4.RECORD,p.G4.PAUSE,"log","wrapLogger"],v=["setErrorHandler","finished","addToTrace","addRelease"];var m=r(1863),b=r(2614),y=r(993);var w=r(2646),A=r(3434);function R(e,t,r,n){if("object"!=typeof t||!t||"string"!=typeof r||!r||"function"!=typeof t[r])return(0,l.R)(29);const i=function(e){return(e||s.ee).get("logger")}(e),o=(0,A.YM)(i),a=new w.y(s.P);return a.level=n.level,a.customAttributes=n.customAttributes,o.inPlace(t,[r],"wrap-logger-",a),i}function E(){const e=(0,g.pV)();h.forEach((t=>{e[t]=(...r)=>function(t,...r){let n=[];return Object.values(e.initializedAgents).forEach((e=>{e&&e.api?e.exposed&&e.api[t]&&n.push(e.api[t](...r)):(0,l.R)(38,t)})),n.length>1?n:n[0]}(t,...r)}))}const x={};function _(e,t,g=!1){t||(0,c.Ak)(e,"api");const h={};var w=s.ee.get(e),A=w.get("tracer");x[e]=b.g.OFF,w.on(p.G4.REPLAY_RUNNING,(t=>{x[e]=t}));var E="api-",_=E+"ixn-";function N(t,r,n,o){const a=(0,i.Vp)(e);return null===r?delete a.jsAttributes[t]:(0,i.x1)(e,{...a,jsAttributes:{...a.jsAttributes,[t]:r}}),k(E,n,!0,o||null===r?"session":void 0)(t,r)}function T(){}h.log=function(e,{customAttributes:t={},level:r=y.p_.INFO}={}){(0,a.p)(f.xV,["API/log/called"],void 0,n.K.metrics,w),function(e,t,r={},i=y.p_.INFO){(0,a.p)(f.xV,["API/logging/".concat(i.toLowerCase(),"/called")],void 0,n.K.metrics,e),(0,a.p)(y.ET,[(0,m.t)(),t,r,i],void 0,n.K.logging,e)}(w,e,t,r)},h.wrapLogger=(e,t,{customAttributes:r={},level:i=y.p_.INFO}={})=>{(0,a.p)(f.xV,["API/wrapLogger/called"],void 0,n.K.metrics,w),R(w,e,t,{customAttributes:r,level:i})},v.forEach((e=>{h[e]=k(E,e,!0,"api")})),h.addPageAction=k(E,"addPageAction",!0,n.K.genericEvents),h.setPageViewName=function(t,r){if("string"==typeof t)return"/"!==t.charAt(0)&&(t="/"+t),(0,o.f)(e).customTransaction=(r||"http://custom.transaction")+t,k(E,"setPageViewName",!0)()},h.setCustomAttribute=function(e,t,r=!1){if("string"==typeof e){if(["string","number","boolean"].includes(typeof t)||null===t)return N(e,t,"setCustomAttribute",r);(0,l.R)(40,typeof t)}else(0,l.R)(39,typeof e)},h.setUserId=function(e){if("string"==typeof e||null===e)return N("enduser.id",e,"setUserId",!0);(0,l.R)(41,typeof e)},h.setApplicationVersion=function(e){if("string"==typeof e||null===e)return N("application.version",e,"setApplicationVersion",!1);(0,l.R)(42,typeof e)},h.start=()=>{try{(0,a.p)(f.xV,["API/start/called"],void 0,n.K.metrics,w),w.emit("manual-start-all")}catch(e){(0,l.R)(23,e)}},h[p.G4.RECORD]=function(){(0,a.p)(f.xV,["API/recordReplay/called"],void 0,n.K.metrics,w),(0,a.p)(p.G4.RECORD,[],void 0,n.K.sessionReplay,w)},h[p.G4.PAUSE]=function(){(0,a.p)(f.xV,["API/pauseReplay/called"],void 0,n.K.metrics,w),(0,a.p)(p.G4.PAUSE,[],void 0,n.K.sessionReplay,w)},h.interaction=function(e){return(new T).get("object"==typeof e?e:{})};const S=T.prototype={createTracer:function(e,t){var r={},i=this,o="function"==typeof t;return(0,a.p)(f.xV,["API/createTracer/called"],void 0,n.K.metrics,w),g||(0,a.p)(_+"tracer",[(0,m.t)(),e,r],i,n.K.spa,w),function(){if(A.emit((o?"":"no-")+"fn-start",[(0,m.t)(),i,o],r),o)try{return t.apply(this,arguments)}catch(e){const t="string"==typeof e?new Error(e):e;throw A.emit("fn-err",[arguments,this,t],r),t}finally{A.emit("fn-end",[(0,m.t)()],r)}}}};function k(e,t,r,i){return function(){return(0,a.p)(f.xV,["API/"+t+"/called"],void 0,n.K.metrics,w),i&&(0,a.p)(e+t,[(0,m.t)(),...arguments],r?null:this,i,w),r?void 0:this}}function I(){r.e(296).then(r.bind(r,8778)).then((({setAPI:t})=>{t(e),(0,c.Ze)(e,"api")})).catch((e=>{(0,l.R)(27,e),w.abort()}))}return["actionText","setName","setAttribute","save","ignore","onEnd","getContext","end","get"].forEach((e=>{S[e]=k(_,e,void 0,g?n.K.softNav:n.K.spa)})),h.setCurrentRouteName=g?k(_,"routeName",void 0,n.K.softNav):k(E,"routeName",!0,n.K.spa),h.noticeError=function(t,r){"string"==typeof t&&(t=new Error(t)),(0,a.p)(f.xV,["API/noticeError/called"],void 0,n.K.metrics,w),(0,a.p)("err",[t,(0,m.t)(),!1,r,!!x[e]],void 0,n.K.jserrors,w)},d.RI?(0,u.GG)((()=>I()),!0):I(),h}var N=r(9417),T=r(8122);const S={accountID:void 0,trustKey:void 0,agentID:void 0,licenseKey:void 0,applicationID:void 0,xpid:void 0},k={};var I=r(5284);const j=e=>{const t=e.startsWith("http");e+="/",r.p=t?e:"https://"+e};let O=!1;function P(e,t={},r,n){let{init:a,info:c,loader_config:u,runtime:l={},exposed:f=!0}=t;l.loaderType=r;const p=(0,g.pV)();c||(a=p.init,c=p.info,u=p.loader_config),(0,N.xN)(e.agentIdentifier,a||{}),function(e,t){if(!e)throw new Error("All loader-config objects require an agent identifier!");k[e]=(0,T.a)(t,S);const r=(0,g.nY)(e);r&&(r.loader_config=k[e])}(e.agentIdentifier,u||{}),c.jsAttributes??={},d.bv&&(c.jsAttributes.isWorker=!0),(0,i.x1)(e.agentIdentifier,c);const h=(0,N.D0)(e.agentIdentifier),v=[c.beacon,c.errorBeacon];O||(h.proxy.assets&&(j(h.proxy.assets),v.push(h.proxy.assets)),h.proxy.beacon&&v.push(h.proxy.beacon),E(),(0,g.US)("activatedFeatures",I.B),e.runSoftNavOverSpa&&=!0===h.soft_navigations.enabled&&h.feature_flags.includes("soft_nav")),l.denyList=[...h.ajax.deny_list||[],...h.ajax.block_internal?v:[]],l.ptid=e.agentIdentifier,(0,o.V)(e.agentIdentifier,l),e.ee=s.ee.get(e.agentIdentifier),void 0===e.api&&(e.api=_(e.agentIdentifier,n,e.runSoftNavOverSpa)),void 0===e.exposed&&(e.exposed=f),O=!0}},8374:(e,t,r)=>{r.nc=(()=>{try{return document?.currentScript?.nonce}catch(e){}return""})()},860:(e,t,r)=>{"use strict";r.d(t,{K:()=>n,P:()=>i});const n={ajax:"ajax",genericEvents:"generic_events",jserrors:"jserrors",logging:"logging",metrics:"metrics",pageAction:"page_action",pageViewEvent:"page_view_event",pageViewTiming:"page_view_timing",sessionReplay:"session_replay",sessionTrace:"session_trace",softNav:"soft_navigations",spa:"spa"},i={[n.pageViewEvent]:1,[n.pageViewTiming]:2,[n.metrics]:3,[n.jserrors]:4,[n.spa]:5,[n.ajax]:6,[n.sessionTrace]:7,[n.softNav]:8,[n.sessionReplay]:9,[n.logging]:10,[n.genericEvents]:11}}},n={};function i(e){var t=n[e];if(void 0!==t)return t.exports;var o=n[e]={exports:{}};return r[e](o,o.exports,i),o.exports}i.m=r,i.d=(e,t)=>{for(var r in t)i.o(t,r)&&!i.o(e,r)&&Object.defineProperty(e,r,{enumerable:!0,get:t[r]})},i.f={},i.e=e=>Promise.all(Object.keys(i.f).reduce(((t,r)=>(i.f[r](e,t),t)),[])),i.u=e=>"nr-rum-1.270.3.min.js",i.o=(e,t)=>Object.prototype.hasOwnProperty.call(e,t),e={},t="NRBA-1.270.3.PROD:",i.l=(r,n,o,a)=>{if(e[r])e[r].push(n);else{var s,c;if(void 0!==o)for(var u=document.getElementsByTagName("script"),d=0;d<u.length;d++){var l=u[d];if(l.getAttribute("src")==r||l.getAttribute("data-webpack")==t+o){s=l;break}}if(!s){c=!0;var f={296:"sha512-+XpdgZ+gEYnk9OOgChKNZ/0lZSiLx1k1ClT5AyRfmPUS7RA6ui+/mJk7HeT5ApSalHfgyDy+DlchnHFWk30nSQ=="};(s=document.createElement("script")).charset="utf-8",s.timeout=120,i.nc&&s.setAttribute("nonce",i.nc),s.setAttribute("data-webpack",t+o),s.src=r,0!==s.src.indexOf(window.location.origin+"/")&&(s.crossOrigin="anonymous"),f[a]&&(s.integrity=f[a])}e[r]=[n];var g=(t,n)=>{s.onerror=s.onload=null,clearTimeout(p);var i=e[r];if(delete e[r],s.parentNode&&s.parentNode.removeChild(s),i&&i.forEach((e=>e(n))),t)return t(n)},p=setTimeout(g.bind(null,void 0,{type:"timeout",target:s}),12e4);s.onerror=g.bind(null,s.onerror),s.onload=g.bind(null,s.onload),c&&document.head.appendChild(s)}},i.r=e=>{"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},i.p="https://js-agent.newrelic.com/",(()=>{var e={840:0,374:0};i.f.j=(t,r)=>{var n=i.o(e,t)?e[t]:void 0;if(0!==n)if(n)r.push(n[2]);else{var o=new Promise(((r,i)=>n=e[t]=[r,i]));r.push(n[2]=o);var a=i.p+i.u(t),s=new Error;i.l(a,(r=>{if(i.o(e,t)&&(0!==(n=e[t])&&(e[t]=void 0),n)){var o=r&&("load"===r.type?"missing":r.type),a=r&&r.target&&r.target.src;s.message="Loading chunk "+t+" failed.\n("+o+": "+a+")",s.name="ChunkLoadError",s.type=o,s.request=a,n[1](s)}}),"chunk-"+t,t)}};var t=(t,r)=>{var n,o,[a,s,c]=r,u=0;if(a.some((t=>0!==e[t]))){for(n in s)i.o(s,n)&&(i.m[n]=s[n]);if(c)c(i)}for(t&&t(r);u<a.length;u++)o=a[u],i.o(e,o)&&e[o]&&e[o][0](),e[o]=0},r=self["webpackChunk:NRBA-1.270.3.PROD"]=self["webpackChunk:NRBA-1.270.3.PROD"]||[];r.forEach(t.bind(null,0)),r.push=t.bind(null,r.push.bind(r))})(),(()=>{"use strict";i(8374);var e=i(944),t=i(6344),r=i(9566);class n{agentIdentifier;constructor(e=(0,r.LA)(16)){this.agentIdentifier=e}#e(t,...r){if("function"==typeof this.api?.[t])return this.api[t](...r);(0,e.R)(35,t)}addPageAction(e,t){return this.#e("addPageAction",e,t)}setPageViewName(e,t){return this.#e("setPageViewName",e,t)}setCustomAttribute(e,t,r){return this.#e("setCustomAttribute",e,t,r)}noticeError(e,t){return this.#e("noticeError",e,t)}setUserId(e){return this.#e("setUserId",e)}setApplicationVersion(e){return this.#e("setApplicationVersion",e)}setErrorHandler(e){return this.#e("setErrorHandler",e)}finished(e){return this.#e("finished",e)}addRelease(e,t){return this.#e("addRelease",e,t)}start(e){return this.#e("start",e)}recordReplay(){return this.#e(t.G4.RECORD)}pauseReplay(){return this.#e(t.G4.PAUSE)}addToTrace(e){return this.#e("addToTrace",e)}setCurrentRouteName(e){return this.#e("setCurrentRouteName",e)}interaction(){return this.#e("interaction")}log(e,t){return this.#e("log",e,t)}wrapLogger(e,t,r){return this.#e("wrapLogger",e,t,r)}}var o=i(860),a=i(9417);const s=Object.values(o.K);function c(e){const t={};return s.forEach((r=>{t[r]=function(e,t){return!0===(0,a.gD)(t,"".concat(e,".enabled"))}(r,e)})),t}var u=i(7603);var d=i(1687),l=i(4234),f=i(5289),g=i(6154),p=i(384);const h=e=>g.RI&&!0===(0,a.gD)(e,"privacy.cookies_enabled");function v(e){return!!(0,p.dV)().o.MO&&h(e)&&!0===(0,a.gD)(e,"session_trace.enabled")}var m=i(6389);class b extends l.W{constructor(e,t,r=!0){super(e.agentIdentifier,t),this.auto=r,this.abortHandler=void 0,this.featAggregate=void 0,this.onAggregateImported=void 0,!1===e.init[this.featureName].autoStart&&(this.auto=!1),this.auto?(0,d.Ak)(e.agentIdentifier,t):this.ee.on("manual-start-all",(0,m.J)((()=>{(0,d.Ak)(e.agentIdentifier,this.featureName),this.auto=!0,this.importAggregator(e)})))}importAggregator(t,r={}){if(this.featAggregate||!this.auto)return;let n;this.onAggregateImported=new Promise((e=>{n=e}));const a=async()=>{let a;try{if(h(this.agentIdentifier)){const{setupAgentSession:e}=await i.e(296).then(i.bind(i,3861));a=e(this.agentIdentifier)}}catch(t){(0,e.R)(20,t),this.ee.emit("internal-error",[t]),this.featureName===o.K.sessionReplay&&this.abortHandler?.()}try{if(t.sharedAggregator)await t.sharedAggregator;else{t.sharedAggregator=i.e(296).then(i.bind(i,5987));const{Aggregator:e}=await t.sharedAggregator;t.sharedAggregator=new e}if(!this.#t(this.featureName,a))return(0,d.Ze)(this.agentIdentifier,this.featureName),void n(!1);const{lazyFeatureLoader:e}=await i.e(296).then(i.bind(i,6103)),{Aggregate:o}=await e(this.featureName,"aggregate");this.featAggregate=new o(t,r),n(!0)}catch(t){(0,e.R)(34,t),this.abortHandler?.(),(0,d.Ze)(this.agentIdentifier,this.featureName,!0),n(!1),this.ee&&this.ee.abort()}};g.RI?(0,f.GG)((()=>a()),!0):a()}#t(e,t){switch(e){case o.K.sessionReplay:return v(this.agentIdentifier)&&!!t;case o.K.sessionTrace:return!!t;default:return!0}}}var y=i(6630);class w extends b{static featureName=y.T;constructor(e,t=!0){super(e,y.T,t),this.importAggregator(e)}}var A=i(9908),R=i(2843),E=i(3878),x=i(782),_=i(1863);class N extends b{static featureName=x.T;constructor(e,t=!0){super(e,x.T,t),g.RI&&((0,R.u)((()=>(0,A.p)("docHidden",[(0,_.t)()],void 0,x.T,this.ee)),!0),(0,E.sp)("pagehide",(()=>(0,A.p)("winPagehide",[(0,_.t)()],void 0,x.T,this.ee))),this.importAggregator(e))}}var T=i(3969);class S extends b{static featureName=T.TZ;constructor(e,t=!0){super(e,T.TZ,t),this.importAggregator(e)}}new class extends n{constructor(t,r){super(r),g.gm?(this.features={},(0,p.bQ)(this.agentIdentifier,this),this.desiredFeatures=new Set(t.features||[]),this.desiredFeatures.add(w),this.runSoftNavOverSpa=[...this.desiredFeatures].some((e=>e.featureName===o.K.softNav)),(0,u.j)(this,t,t.loaderType||"agent"),this.run()):(0,e.R)(21)}get config(){return{info:this.info,init:this.init,loader_config:this.loader_config,runtime:this.runtime}}run(){try{const t=c(this.agentIdentifier),r=[...this.desiredFeatures];r.sort(((e,t)=>o.P[e.featureName]-o.P[t.featureName])),r.forEach((r=>{if(!t[r.featureName]&&r.featureName!==o.K.pageViewEvent)return;if(this.runSoftNavOverSpa&&r.featureName===o.K.spa)return;if(!this.runSoftNavOverSpa&&r.featureName===o.K.softNav)return;const n=function(e){switch(e){case o.K.ajax:return[o.K.jserrors];case o.K.sessionTrace:return[o.K.ajax,o.K.pageViewEvent];case o.K.sessionReplay:return[o.K.sessionTrace];case o.K.pageViewTiming:return[o.K.pageViewEvent];default:return[]}}(r.featureName).filter((e=>!(e in this.features)));n.length>0&&(0,e.R)(36,{targetFeature:r.featureName,missingDependencies:n}),this.features[r.featureName]=new r(this)}))}catch(t){(0,e.R)(22,t);for(const e in this.features)this.features[e].abortHandler?.();const r=(0,p.Zm)();delete r.initializedAgents[this.agentIdentifier]?.api,delete r.initializedAgents[this.agentIdentifier]?.features,delete this.sharedAggregator;return r.ee.get(this.agentIdentifier).abort(),!1}}}({features:[w,N,S],loaderType:"lite"})})()})();</script>
<meta name="document-type" content="Public">
<meta name="document-rating" content="Safe for Kids">
<meta name="robots" content="ALL, INDEX, FOLLOW">
<meta name="googlebot" content="index, follow">
<meta name="Expires" content="never">
<meta name="coverage" content="Worldwide">
<meta name="distribution" content="Global">
<meta name="rating" content="General">
<meta name="revisit-after" content="7 days">
<meta name="target" content="all">
<meta name="HandheldFriendly" content="True">
<meta name="mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-capable" content="yes">
    <link rel="apple-touch-icon" href="https://plk.websites.co.in/files/2078374/favicon/favicon.png?v=2071154643"/>


<meta name="theme-color" content="#f2b531">
<meta name="viewport" content="width=device-width">
<meta name="title" content="Aplus in  Junagadh">
<meta name="description" content="[hwllookwcjoihciuvghivgrfuybgrhv">
<meta name="author" content="Aplus">
<meta name="keywords" content="Aplus,Aplus in Junagadh,Aplus in Gujarat,Aplus in India,Aplus in LOCAL BUSINESS">


<meta name="csrf-token" content="1d14FHWnGckdws1i9ElWDOIJ04pQn8oJHY556cov">



<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Aplus in  Junagadh">
<meta name="twitter:image" content="https://plk.websites.co.in/files/2078374/business/logo/logo-747113528.jpeg">
<meta name="twitter:image:alt" content="Aplus in  Junagadh">
<meta name="twitter:description" content="[hwllookwcjoihciuvghivgrfuybgrhv">



<meta property="og:site_name" content="plk">
<meta property="og:type" content="website">
<meta property="og:title" content="Aplus in  Junagadh">
<meta property="og:description" content="[hwllookwcjoihciuvghivgrfuybgrhv">
<meta property="og:image" content="https://plk.websites.co.in/files/2078374/business/logo/logo-747113528.jpeg">
<meta property="og:url" content="https://plk.websites.co.in">




<meta name="geo.position" content="21.519;70.456">
<meta name="geo.placename" content="Junagadh">
<meta name="geo.region" content="IN">
<!-- Favicon -->
    <link rel="icon" href="https://plk.websites.co.in/files/2078374/favicon/favicon.png?v=805624916" type="image/png" />
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width">
  <title>Aimage</title>
  <style>
    @import url("https://fonts.googleapis.com/css2?family=Nunito:wght@500&display=swap");

    * {
      font-family: "Nunito", Arial, sans-serif;
      color: black;
    }

    

    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(to right, #667eea, #764ba2);
    }

    header {
      min-width: 40%;
      max-width: 60%;
      margin: 0rem auto;
      background-color: #333;
      text-align: center;
      padding: 0.5rem;
      border-radius: 0px 0px 20px 20px;
      box-shadow: 0 0 80px rgba(255, 255, 255, 0.1);
    }

    main {
      min-width: 40%;
      max-width: 60%;
      margin: 2rem auto;
      padding: 0.5rem;
      background: linear-gradient(to right, #667eea, #764ba2);
      border-radius: 20px;
      box-shadow: 0 0 80px rgba(255, 255, 255, 0.1);
    }

    .generator {
      text-align: center;
    }

    .input {
      margin-bottom: 1rem;
    }

    .promptBox {
      width: 95%;
      padding: 0.5rem;
      border-style: none;
      border-radius: 20px;
    }

    .heightWidth {
      width: 40%;
      padding: 0.5rem;
      border-style: none;
      margin-bottom: 1rem;
    }

    #hInput {
      border-radius: 20px 4px 4px 20px;
    }

    #wInput {
      border-radius: 4px 20px 20px 4px;
    }

    button {
      background-color: #0074d9;
      color: white;
      padding: 0.5rem 1rem;
      border: none;
      cursor: pointer;
      border-radius: 8px;
      box-shadow: 0 0 80px rgba(0, 116, 217, 0.4);
    }

    #dlButton {
      background-color: #0074d9;
      color: white;
      padding: 0.5rem 1rem;
      border: none;
      cursor: pointer;
      box-shadow: 0 0 80px rgba(0, 116, 217, 0.4);
      border-radius: 20px;
      display: none;
      text-decoration: none;
    }

    #generate {
      position: fixed;
      bottom: 20px;
      left: 50%;
      transform: translateX(-50%);
      height: 40px;
      width: 80%;
      background-color: #0074d9;
      color: white;
      padding: 0.5rem 1rem;
      border: none;
      cursor: pointer;
      border-radius: 8px;
      box-shadow: 0 0 80px rgba(0, 116, 217, 0.5);
      transition: opacity 0.333s;
    }

    #generate.hide {
      opacity: 0;
      pointer-events: none;
    }

    .output {
      text-align: center;
    }

    #image-container img {
      max-width: 100%;
      height: auto;
      margin-top: 1rem;
      border-radius: 20px;
    }

    .discreteLink {
      color: whitesmoke;
      text-decoration: underline;
      text-decoration-style: dotted;
      text-decoration-color: #0074d9;
    }

    #generatedText {
      display: none;
    }

    .loader {
      border: 6px solid black;
      border-top: 6px solid white;
      border-radius: 50%;
      width: 50px;
      height: 50px;
      animation: spin 1s linear infinite;
      margin: 0 auto;
      margin-top: 1rem;
      display: none;
    }

    @keyframes spin {
      0% {
        transform: rotate(0deg);
      }

      100% {
        transform: rotate(360deg);
      }
    }
  </style>
  <script src="https://cdn.gravitec.net/storage/c23a032ef396b3eb1f18fde3fa0c6d5b/client.js" async></script>
<style>
.gfhfg {
    font-family: 'Megrim';
    font-style: normal;
    font-weight: 400;
    src: local('Megrim'),
    url('static/resources/fonts/megrim-v10-latin-regular.ttf') format('truetype'),
}
</style>
</head>
<body>
<center><a href="https://3rsuux.mimo.run/index.html"><img src="https://i.ibb.co/j3TH1Yr/Whats-App-Image-2024-10-28-at-4-07-24-PM-photoaidcom-cropped.png" height="90" width="90"></a></center>
<div style = "display: flex; justify-content:flex-end"><a href="https://klm31x.mimo.run/index.html"><button style=“background-color: COLOR NAME;border-color:COLOR NAME;color:COLOR NAME”>Sign up</button></a></div>
<div class="gfhfg">
<p></p>
</div>
  <main>
    <div class="generator">
      <div class="input">
        <br>
        <input class="promptBox" type="text" id="prompt" placeholder="Enter your img name here">
      </div>
      <div>
        <input class="heightWidth" type="text" id="hInput" placeholder="Height">
        <input class="heightWidth" type="text" id="wInput" placeholder="Width">
      </div>
      <br>
    </div>
    <div>
      <button id="generate">Generate Image</button>
    </div>
    <div class="output">
      <h2 id="generatedText">Generated Image:</h2>
      <div id="loading-spinner" class="loader"></div>
      <div id="image-container"></div>
      <div id="utilities">
        <a id="dlButton" href="">Download</a>
      </div>
    </div>
  </main>

  <script>
    document.addEventListener("DOMContentLoaded", function() {
      const generateButton = document.getElementById("generate");
      const promptInput = document.getElementById("prompt");
      const heightInput = document.getElementById("hInput");
      const widthInput = document.getElementById("wInput");
      const imageContainer = document.getElementById("image-container");
      const loadingSpinner = document.getElementById("loading-spinner");
      const genText = document.getElementById("generatedText");
      const dlButton = document.getElementById("dlButton");

      generateButton.addEventListener("click", function() {
        var description = promptInput.value ?
          encodeURIComponent(promptInput.value) :
          "beautiful%20landscape";
        const randomSeed = Math.floor(Math.random() * 1000000000);
        const heightA = heightInput.value ? parseInt(heightInput.value) : 360;
        const widthA = widthInput.value ? parseInt(widthInput.value) : 480;
        loadingSpinner.style.display = "block";
        genText.style.display = "none";
        generateButton.classList.add("hide");
        const imageUrl = `https://image.pollinations.ai/prompt/${description}?nologo=1&seed=${randomSeed}&height=${heightA}&width=${widthA}`;
        console.log("URL: " + imageUrl);
        const image = document.createElement("img");
        image.onload = function() {
          loadingSpinner.style.display = "none";
          genText.style.display = "block";
          dlButton.setAttribute("href", imageUrl);
          dlButton.style.display = "block";
          generateButton.classList.remove("hide");
          imageContainer.innerHTML = "";
          imageContainer.appendChild(image);
        };
        image.onerror = function() {
          loadingSpinner.style.display = "none";
          alert("Failed to load image. Please try again.");
          generateButton.classList.remove("hide");
        };
        image.src = imageUrl;
      });
    });
  </script>
  <script>
// Prevent keyboard key
$(document).keydown(function (e) {
if (e.keyCode == 123) { // Prevent F12
return false;
} else if (e.ctrlKey && e.shiftKey && e.keyCode == 73) { // Prevent Ctrl+Shift+I
return false;
} else if (e.ctrlKey && e.keyCode == 85) { // Prevent Ctrl+u
return false;
}
});
    </script>
    <script>
    alert(e.keyCode);
    }*/
    document.onkeydown = function(e) {
            if (e.ctrlKey && (e.keyCode === 67 || e.keyCode === 86 || e.keyCode === 85 || e.keyCode === 117)) {//Alt+c, Alt+v will also be disabled sadly.
                alert('not allowed');
            }
            return false;
    };
    </script>
</body>
<body onkeypress="return disableCtrlKeyCombination(event);" onkeydown="return disableCtrlKeyCombination(event);">
</body>
</Html>
