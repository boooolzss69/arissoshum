function login() {
  window.location.href = "dashboard.html";
}

function previewImage(event) {
  const preview = document.getElementById("preview");
  preview.src = URL.createObjectURL(event.target.files[0]);

  // Simulasi klasifikasi AI
  const hasil = [
    {
      jenis: "Sampah Plastik",
      edukasi: "Plastik dapat didaur ulang menjadi pot tanaman atau tas. Jangan dibakar!"
    },
    {
      jenis: "Sampah Organik",
      edukasi: "Sampah organik bisa dijadikan kompos untuk pupuk alami."
    },
    {
      jenis: "Sampah Kertas",
      edukasi: "Kertas dapat didaur ulang hingga 5 kali. Kurangi penggunaan kertas."
    }
  ];

  const random = hasil[Math.floor(Math.random() * hasil.length)];

  document.getElementById("classification").innerText =
    "Jenis Sampah: " + random.jenis;

  document.getElementById("education").innerText =
    "Edukasi: " + random.edukasi;
}
