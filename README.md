# Firefox Privacy Setup

- 본 목록에 있는 내용을 수행했을 때 일부 사이트나 결제 프로세스가 작동되지 않을 수 있습니다.
- Some sites or payment processes might not work when you do something on this list.

## reference

ref1. https://web.archive.org/web/20221013104259/https://chrisx.xyz/blog/yet-another-firefox-hardening-guide/

ref2. https://gogilove.wordpress.com/2019/05/02/firefox/


## in about:config

### Isolate cookie
- privacy.firstparty.isolate `true`

### Disable URL speculative connect
- browser.urlbar.speculativeConnect.enabled `false`

### Resist fingerprint
- privacy.resistFingerprinting `true`
  
### Disable telemetry
- browser.newtabpage.activity-stream.feeds.telemetry `false`
- browser.tabs.crashReporting.sendReport `false`
- toolkit.telemetry.enabled `false`
- toolkit.telemetry.server `leave it empty`
- toolkit.telemetry.unified `false`

### Disable Pocket
- browser.newtabpage.activity-stream.feeds.discoverystreamfeed `false`
- browser.newtabpage.activity-stream.feeds.section.topstories `false`
- browser.newtabpage.activity-stream.section.highlights.includePocket `false`
- browser.newtabpage.activity-stream.showSponsored `false`
- extensions.pocket.enabled `false`

### Disable prefetching
- network.dns.disablePrefetch `true`
- network.prefetch-next `false`

### Disable JavaScript in PDF
- pdfjs.enableScripting `false`

### Harden SSL preferences 
- Change security.ssl.require_safe_negotiation `true`

### Disable Firefox account features
- identity.fxaccounts.enabled `false`

### Disable geolocation support
- geo.enabled `false`

### Disable notification support
- dom.webnotifications.enabled `false`

### Disable WebRTC
- media.peerconnection.enabled `false`
- media.navigator.enabled `false`

### Disable WebGL
- webgl.disabled `true`


