This is a local, client-side only web "proxy" that was created by dinguschan on Feb 28, 2024. Note that this is not a true proxy, because it is not routing your internet traffic through any external servers. Nonetheless, if you open any website through this file, it will not appear in your search history, not be affected by any blockers or trackers, but your screen can still be seen by admin controlled spyware (GoGuardian, Securly, etc.) The project works by using the fetch function in Javascript to fetch the HTML, CSS, and JS elements from a website, then displays it on this page. Keep in mind that this is a very basic demonstration of this method, so following links in the website and non HTTPS websites are not supported. If you are interested, you can find the project on GitHub <a href="https://github.com/maximusweeseman/local-webproxy"><b>here</b></a>. I will probably not keep maintaining this demonstration past update 1.2, so I strongly urge you to use a better method to do your internet tomfoolery. In the meantime, dinguschan out. 👋

USAGE INSTRUCTIONS: Just download the HTML file lol. Thats why its a clientside only LOCAL "proxy." IF you are too paranoid to have this file on your computer, you can copy and paste this into your url bar instead :D

■□■□■□■□■□■■□■□■□■□■□■■□■□■□■□■□■■□■□■□■□■□■■□■□■□■□■□■■□■□■□■□■□■■□■□■□■□■□■■□■□■□

_**[THIS PAGE DOES NOT WORK. PLEASE DOWNLOAD THE LOCAL FILE INSTEAD]**_

data:text/html, <script> function getHtml(file){ return new Promise((resolve) => { fetch(file) .then((response) => { return response.text(); }) .then((html) => { resolve(html); }); }); } async function start(){ var html=await getHtml('https://raw.githubusercontent.com/maximusweeseman/local-webproxy/main/index.html'); html=html.toString(); console.log(html); document.body.innerHTML=html; } start(); </script>

■□■□■□■□■□■■□■□■□■□■□■■□■□■□■□■□■■□■□■□■□■□■■□■□■□■□■□■■□■□■□■□■□■■□■□■□■□■□■■□■□■□
