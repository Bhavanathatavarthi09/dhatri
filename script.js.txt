function sendWhatsApp(event) {
  event.preventDefault();

  let name = document.getElementById("name").value;
  let email = document.getElementById("email").value;
  let product = document.getElementById("product").value;
  let message = document.getElementById("message").value;

  // CHANGE THIS NUMBER TO YOUR WHATSAPP NUMBER
  let phone = "919999999999";

  let text = `Hello, I want to order from Dhatri Collections:%0A
Name: ${name}%0A
Email: ${email}%0A
Product: ${product}%0A
Message: ${message}`;

  let url = `https://wa.me/${phone}?text=${text}`;

  window.open(url, "_blank");
}
