

<head>
  <script src="/cdn-cgi/apps/head/aqhzBqkyhgXFT9tYquvCBE2xpuY.js"></script>
  <style>
    div a img {
      visibility: hidden;
    }
  </style>
  <meta name='viewport' content='width=device-width, initial-scale=1.0' />
  <meta name="referrer" content="no-referrer" />
  <script src='https://cdnjs.cloudflare.com/ajax/libs/shaka-player/4.1.1/shaka-player.ui.min.js'
    crossorigin='anonymous'></script>
  <link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/shaka-player/4.1.1/controls.min.css'
    crossorigin='anonymous' />
  <script async src='/cdn-cgi/challenge-platform/h/g/scripts/invisible.js?cb=6ebfddfd6fa3499c'></script>
</head>

<body>
  <script>!function (a, b, c, d, e, f) {a.ddjskey = e; a.ddoptions = f || null; var m = b.createElement(c), n = b.getElementsByTagName(c)[0]; m.async = 1, m.src = d, n.parentNode.insertBefore(m, n)}(window, document, "script", "https://js.datadome.co/tags.js", "99B1C08278137CE22ADB60CE8DE020", {"ajaxListenerPath": true});</script>

  <body bgcolor='black' style='margin:0' oncontextmenu='return false' onkeydown='return false'
    onmousedown='return false'>
    <script>!function (a, b, c, d, e, f) {a.ddjskey = e; a.ddoptions = f || null; var m = b.createElement(c), n = b.getElementsByTagName(c)[0]; m.async = 1, m.src = d, n.parentNode.insertBefore(m, n)}(window, document, "script", "https://js.datadome.co/tags.js", "99B1C08278137CE22ADB60CE8DE020", {"ajaxListenerPath": true});</script>
    <div data-shaka-player-container
      style='position:absolute;z-index: -1;top: 0;left: 0;width: 100%; height: 100%;object-fit: cover;'><video autoplay poster="https://s.id/1x8HU" data-shaka-player id='video' style='width:100%;height:100%;'></video></div>
    <script>
      async function init() {
        const video = document.getElementById('video');
        const ui = video['ui'];
        const controls = ui.getControls();
        const player = controls.getPlayer();
        player.configure({
          drm: {
            clearKeys: {
              // 'key-id-in-hex': 'key-in-hex',
              'a9e0ecea640959c6aec904a1f34934a5': '284ea8e5fa0de4bc90c17c21148dbdea'
            }
          }
        });
        //player.configure({drm:{servers:{'com.widevine.alpha':'https://license.dstv.com/widevine/getLicense?CrmId=afl&AccountId=afl&ContentId=SH2&SessionId=D3C00F885C24B9C6&Ticket=C839A8D71AB94299'}}}); 
        window.player = player;
        window.ui = ui;
        player.addEventListener('error', onPlayerErrorEvent);
        controls.addEventListener('error', onUIErrorEvent);
        try {
          await player.load('https://director.streaming.telia.com/tvm-packager-prod/group3/60ae4bff1522bd2d466954df/manifest.mpd');
          console.log('The video has now been loaded!');
        } catch (error) {onPlayerError(error);}
      }
      function onPlayerErrorEvent(errorEvent) {onPlayerError(event.detail);}
      function onPlayerError(error) {console.error('Error code', error.code, 'object', error);}
      function onUIErrorEvent(errorEvent) {onPlayerError(event.detail);}
      function initFailed(errorEvent) {console.error('Unable to load the UI library!');}
      document.addEventListener('shaka-ui-loaded', init);
      document.addEventListener('shaka-ui-load-failed', initFailed);
    </script>
    <script type='text/javascript' src='https://encrypt2.skycdn.ga/udp/Counter'></script>
    <script
      type="text/javascript">(function () {window['__CF$cv$params'] = {r: '6ebfddfd6fa3499c', m: 'D4YJv6au4IB.PA2DqTLxZStJydWh51fiwv2G9eC_8Gk-1647290874-0-AYjwUV5YDhzDCl2C9r7Xi8tcRCaEcQTbCAMGCeTNqDvB45L3MnGBdkKHu6G387dXhgYcctN3ANz21D9fu1HhsRAcyKR0VCGqS9aNi6PQ8MvMDWfoO6WhJhqlukHMDXtYfg==', s: [0x6c6fafcade, 0x9f5e65094f], u: '/cdn-cgi/challenge-platform/h/g'}})();</script>
    <script defer
      src="https://static.cloudflareinsights.com/beacon.min.js/v652eace1692a40cfa3763df669d7439c1639079717194"
      integrity="sha512-Gi7xpJR8tSkrpF7aordPZQlW2DLtzUlZcumS8dMQjwDHEnw9I7ZLyiOj/6tZStRBGtGgN6ceN6cMH8z7etPGlw=="
      data-cf-beacon='{"rayId":"6ebfddfd6fa3499c","version":"2021.12.0","r":1,"token":"a919438182254588b33b5297605b9ab4","si":100}'
      crossorigin="anonymous"></script>
