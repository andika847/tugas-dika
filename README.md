function hitungGaji(hariHadir, potongan) {
  const gajiPokok = 5000000;
  const tambahanHadir = 200000;
  const bonus = 500000;

  let totalGaji = gajiPokok;
  totalGaji += hariHadir * tambahanHadir;

  if (hariHadir > 20) {
    totalGaji += bonus;
  }

  if (potongan > 200000) {
    totalGaji -= potongan;
  }

  return totalGaji;
}

// Contoh penggunaan
console.log(hitungGaji(15, 0)); // Output: 8000000
console.log(hitungGaji(25, 0)); // Output: 10500000
console.log(hitungGaji(20, 500000)); // Output: 8500000
