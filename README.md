:

🛡️ Sistem Keamanan Brankas & Monitoring Suhu (Tanpa Breadboard)
Proyek ini adalah simulasi sistem keamanan brankas pintar yang dibangun menggunakan Arduino Uno di platform Tinkercad. Sistem ini mengintegrasikan kontrol akses fisik (Servo), sistem pendingin otomatis (Motor DC), dan monitoring kondisi lingkungan secara real-time (LCD & Sensor Suhu).

🚀 Fitur Utama
Security Access Control: Menggunakan potensiometer untuk mensimulasikan pembukaan kunci brankas melalui Servo Motor.

Real-time Temperature Monitoring: Sensor TMP36 memantau suhu di dalam brankas.

Auto-Cooling System: Motor DC (kipas) akan aktif secara otomatis jika suhu brankas melebihi 35°C untuk mencegah overheat pada komponen di dalam.

Dual Indicator LEDs: LED Hijau menandakan status brankas (Terbuka/Terkunci), dan LED Merah menandakan peringatan suhu tinggi.

Visual Interface: LCD 16x2 I2C menampilkan data suhu dan status keamanan secara presisi.

🛠️ Komponen yang Digunakan
Arduino Uno R3

LCD 16x2 (I2C Module) - Address: 0x26

Motor Driver L293D (Direct Wiring)

Servo Motor

Sensor Suhu TMP36

Potensiometer (10k Ohm)

Motor DC

Baterai 9V (External Power for Motor)

LED Merah & Hijau + Resistor 220 Ohm

🖇️ Diagram Wiring (Highlight)
Salah satu tantangan terbesar dalam proyek ini adalah melakukan Direct Wiring pada IC L293D tanpa menggunakan breadboard untuk menjaga kerapian arus.

Pin 16 L293D: Terhubung ke 5V Arduino (Logic Power).

Pin 8 L293D: Terhubung ke 9V Baterai (Motor Power).

Common Ground: Semua jalur negatif (GND) disatukan ke pin GND Arduino untuk kestabilan sinyal.

💻 Cara Menjalankan
Copy kode program yang ada di file .ino ke IDE Arduino atau Tinkercad.

Pastikan library LiquidCrystal_I2C dan Servo sudah terpasang.

Sesuaikan alamat I2C pada kode (0x26) jika menggunakan perangkat fisik yang berbeda.

Klik Start Simulation.
