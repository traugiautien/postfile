# postfile

  fetch("http://192.168.1.3:3000/list-profiles")
  .then(res => res.json())
  .then(data => console.log("📄 Danh sách profile:", data));
