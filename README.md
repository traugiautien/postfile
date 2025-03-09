# postfile

fetch("http://192.168.1.5:8080/list-profiles")
.then(res => res.json())
.then(data => console.log("📄 Danh sách profile:", data));


let ws = new WebSocket("ws://192.168.1.5:8080");
ws.onopen = () => console.log("Connected!");
ws.onmessage = (msg) => console.log("Received:", msg.data);
ws.onerror = (err) => console.error("Error:", err);
ws.onclose = () => console.log("Disconnected!");

http://192.168.1.5:8080/get-profile/someuser
