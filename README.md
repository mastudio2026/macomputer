export default function MaStudioWebsite() { return ( <div className="min-h-screen bg-gradient-to-b from-slate-950 to-slate-900 text-white font-sans"> {/* Hero Section */} <section className="relative overflow-hidden"> <div className="absolute inset-0 bg-[url('https://images.unsplash.com/photo-1516035069371-29a1b244cc32?q=80&w=1600')] bg-cover bg-center opacity-20"></div> <div className="relative max-w-7xl mx-auto px-6 py-20 grid md:grid-cols-2 gap-10 items-center"> <div> <h1 className="text-5xl md:text-7xl font-extrabold leading-tight"> <span className="text-pink-500">Ma</span>{" "} <span className="text-white">Studio</span> <br /> <span className="text-yellow-400 text-4xl md:text-5xl">& Stationary</span> </h1>

<p className="mt-6 text-lg text-slate-300 leading-relaxed">
          Professional Studio, Online Service, Print, Photocopy,
          Lamination, ID Card Print, Visiting Card, Memo এবং সকল
          প্রকার স্টেশনারি সামগ্রী এক জায়গায়।
        </p>

        <div className="mt-8 flex flex-wrap gap-4">
          <a
            href="tel:01628386555"
            className="bg-pink-600 hover:bg-pink-700 px-6 py-3 rounded-2xl font-semibold shadow-lg"
          >
            📞 Call Now
          </a>

          <a
            href="https://wa.me/8801576570101"
            className="bg-green-600 hover:bg-green-700 px-6 py-3 rounded-2xl font-semibold shadow-lg"
          >
            💬 WhatsApp
          </a>
        </div>
      </div>

      <div className="bg-white/10 backdrop-blur-lg p-6 rounded-3xl shadow-2xl border border-white/10">
        <img
          src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?q=80&w=1200"
          alt="Studio"
          className="rounded-2xl w-full h-[350px] object-cover"
        />
      </div>
    </div>
  </section>

  {/* Services */}
  <section className="max-w-7xl mx-auto px-6 py-16">
    <div className="text-center mb-14">
      <h2 className="text-4xl font-bold text-yellow-400">Our Services</h2>
      <p className="text-slate-300 mt-3">
        দ্রুত ও মানসম্মত সেবা প্রদান করা হয়
      </p>
    </div>

    <div className="grid sm:grid-cols-2 lg:grid-cols-4 gap-6">
      {[
        '📸 Professional Studio',
        '🖨️ Print & Photocopy',
        '💳 ID Card Print',
        '📝 Compose & Typing',
        '📄 Lamination',
        '🎨 Visiting Card Design',
        '🌐 Online Service',
        '✏️ Stationary Products',
      ].map((service, index) => (
        <div
          key={index}
          className="bg-white/10 border border-white/10 rounded-3xl p-6 hover:scale-105 transition duration-300 shadow-lg"
        >
          <h3 className="text-xl font-semibold text-white">{service}</h3>
        </div>
      ))}
    </div>
  </section>

  {/* Studio Highlight */}
  <section className="bg-gradient-to-r from-pink-700 to-purple-700 py-16 px-6">
    <div className="max-w-6xl mx-auto grid md:grid-cols-2 gap-10 items-center">
      <div>
        <img
          src="https://images.unsplash.com/photo-1492691527719-9d1e07e534b4?q=80&w=1200"
          alt="Photography"
          className="rounded-3xl shadow-2xl"
        />
      </div>

      <div>
        <h2 className="text-5xl font-extrabold mb-6">
          📸 Professional Studio
        </h2>

        <p className="text-lg text-pink-100 leading-relaxed mb-6">
          Passport Size Photo, Studio Photography, Family Photo,
          Event Photography এবং Professional Editing সুবিধা।
        </p>

        <ul className="space-y-3 text-lg">
          <li>✅ Passport Size Photo</li>
          <li>✅ Wedding & Event Photography</li>
          <li>✅ Instant Print</li>
          <li>✅ High Quality Editing</li>
        </ul>
      </div>
    </div>
  </section>

  {/* Gallery Section */}
  <section className="max-w-7xl mx-auto px-6 py-20">
    <div className="text-center mb-12">
      <h2 className="text-4xl font-bold text-pink-400">Our Gallery</h2>
      <p className="text-slate-300 mt-3">স্টুডিও ও প্রিন্ট কাজের কিছু নমুনা</p>
    </div>

    <div className="grid md:grid-cols-3 gap-6">
      {[
        'https://images.unsplash.com/photo-1524504388940-b1c1722653e1?q=80&w=1200',
        'https://images.unsplash.com/photo-1516321318423-f06f85e504b3?q=80&w=1200',
        'https://images.unsplash.com/photo-1492691527719-9d1e07e534b4?q=80&w=1200',
      ].map((img, i) => (
        <div key={i} className="overflow-hidden rounded-3xl shadow-2xl">
          <img
            src={img}
            alt="Gallery"
            className="w-full h-[260px] object-cover hover:scale-110 transition duration-500"
          />
        </div>
      ))}
    </div>
  </section>

  {/* Price List */}
  <section className="bg-slate-950 py-16 px-6">
    <div className="max-w-5xl mx-auto">
      <div className="text-center mb-10">
        <h2 className="text-4xl font-bold text-yellow-400">Price List</h2>
        <p className="text-slate-300 mt-3">সাশ্রয়ী মূল্যে উন্নত সেবা</p>
      </div>

      <div className="grid md:grid-cols-2 gap-6">
        {[
          ['Photocopy', '2৳ থেকে'],
          ['Color Print', '15৳ থেকে'],
          ['Lamination', '30৳ থেকে'],
          ['Passport Photo', '80৳ থেকে'],
          ['ID Card Print', '120৳ থেকে'],
          ['Visiting Card', '250৳ থেকে'],
        ].map((item, i) => (
          <div
            key={i}
            className="bg-white/10 rounded-2xl p-5 flex justify-between border border-white/10"
          >
            <span className="text-lg">{item[0]}</span>
            <span className="font-bold text-pink-400">{item[1]}</span>
          </div>
        ))}
      </div>
    </div>
  </section>

  {/* Online Order */}
  <section className="max-w-5xl mx-auto px-6 py-20">
    <div className="bg-gradient-to-r from-purple-700 to-pink-700 rounded-3xl p-10 shadow-2xl">
      <h2 className="text-4xl font-bold text-center mb-8">
        Online Order Form
      </h2>

      <div className="grid gap-5">
        <input
          type="text"
          placeholder="আপনার নাম"
          className="p-4 rounded-2xl bg-white/20 border border-white/20 outline-none"
        />

        <input
          type="text"
          placeholder="মোবাইল নাম্বার"
          className="p-4 rounded-2xl bg-white/20 border border-white/20 outline-none"
        />

        <textarea
          placeholder="আপনার অর্ডার লিখুন"
          rows="5"
          className="p-4 rounded-2xl bg-white/20 border border-white/20 outline-none"
        ></textarea>

        <button className="bg-yellow-400 text-black font-bold py-4 rounded-2xl hover:scale-105 transition">
          Submit Order
        </button>
      </div>
    </div>
  </section>

  {/* Contact */}
  <section className="max-w-6xl mx-auto px-6 py-20">
    <div className="bg-white/10 rounded-3xl p-10 shadow-2xl border border-white/10">
      <h2 className="text-4xl font-bold text-yellow-400 mb-8 text-center">
        Contact Us
      </h2>

      <div className="grid md:grid-cols-2 gap-8 text-lg">
        <div className="space-y-4 text-slate-200">
          <p><strong>📞 Mobile:</strong> 01628386555</p>
          <p><strong>💬 WhatsApp:</strong> 01576570101</p>
          <p><strong>📧 Email:</strong> mastudio626</p>
          <p>
            <strong>📍 Address:</strong> Evercare Hospital Gate,
            Bashundhara R/A, Vatara, Dhaka.
          </p>
        </div>

        <div className="bg-slate-900 rounded-2xl p-6 border border-white/10">
          <h3 className="text-2xl font-semibold mb-4 text-pink-400">
            Why Choose Us?
          </h3>

          <ul className="space-y-3 text-slate-300">
            <li>⭐ Fast Service</li>
            <li>⭐ Affordable Price</li>
            <li>⭐ Professional Studio Setup</li>
            <li>⭐ Quality Print & Design</li>
            <li>⭐ Friendly Customer Support</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  {/* Footer */}
        {/* Customer Reviews */}
  <section className="max-w-6xl mx-auto px-6 py-20">
    <div className="text-center mb-12">
      <h2 className="text-4xl font-bold text-yellow-400">Customer Reviews</h2>
      <p className="text-slate-300 mt-3">আমাদের গ্রাহকদের মতামত</p>
    </div>

    <div className="grid md:grid-cols-3 gap-6">
      {[
        {
          name: 'Rakib Hasan',
          text: 'খুব দ্রুত এবং সুন্দর প্রিন্ট সার্ভিস পেয়েছি।',
        },
        {
          name: 'Nusrat Jahan',
          text: 'স্টুডিও ফটোগ্রাফি এবং আইডি কার্ড প্রিন্ট খুব ভালো।',
        },
        {
          name: 'Tanvir Ahmed',
          text: 'স্টেশনারি জিনিসপত্র ও অনলাইন সার্ভিস একদম অসাধারণ।',
        },
      ].map((review, i) => (
        <div
          key={i}
          className="bg-white/10 p-6 rounded-3xl border border-white/10 shadow-xl"
        >
          <p className="text-slate-300 mb-4">“{review.text}”</p>
          <h4 className="font-bold text-pink-400">⭐ {review.name}</h4>
        </div>
      ))}
    </div>
  </section>

  {/* Facebook & Map */}
  <section className="bg-slate-950 py-20 px-6">
    <div className="max-w-6xl mx-auto grid md:grid-cols-2 gap-8">
      <div className="bg-white/10 p-8 rounded-3xl border border-white/10 shadow-2xl">
        <h2 className="text-3xl font-bold text-blue-400 mb-4">
          Follow Our Facebook Page
        </h2>

        <p className="text-slate-300 mb-6">
          নতুন আপডেট, অফার ও স্টুডিও কাজ দেখতে আমাদের ফেসবুক পেইজ ফলো করুন।
        </p>

        <a
          href="#"
          className="inline-block bg-blue-600 hover:bg-blue-700 px-6 py-3 rounded-2xl font-semibold"
        >
          👍 Visit Facebook Page
        </a>
      </div>

      <div className="bg-white/10 p-8 rounded-3xl border border-white/10 shadow-2xl">
        <h2 className="text-3xl font-bold text-red-400 mb-4">
          Our Location
        </h2>

        <p className="text-slate-300 leading-relaxed">
          📍 Evercare Hospital Gate, Bashundhara R/A,
          Vatara, Dhaka.
        </p>

        <div className="mt-6 rounded-2xl overflow-hidden border border-white/10">
          <iframe
            title="map"
            src="https://maps.google.com/maps?q=Evercare%20Hospital%20Dhaka&t=&z=13&ie=UTF8&iwloc=&output=embed"
            width="100%"
            height="250"
            style={{ border: 0 }}
            loading="lazy"
          ></iframe>
        </div>
      </div>
    </div>
  </section>

  {/* QR & Download */}
  <section className="max-w-6xl mx-auto px-6 py-20">
    <div className="bg-gradient-to-r from-yellow-500 to-orange-500 rounded-3xl p-10 text-black shadow-2xl">
      <div className="grid md:grid-cols-2 gap-10 items-center">
        <div>
          <h2 className="text-4xl font-bold mb-5">Quick Contact & Share</h2>

          <p className="text-lg mb-6">
            QR কোড স্ক্যান করে দ্রুত যোগাযোগ করুন অথবা ওয়েবসাইট শেয়ার করুন।
          </p>

          <div className="flex flex-wrap gap-4">
            <button className="bg-black text-white px-6 py-3 rounded-2xl font-semibold">
              Download Brochure
            </button>

            <button className="bg-white text-black px-6 py-3 rounded-2xl font-semibold">
              Share Website
            </button>
          </div>
        </div>

        <div className="flex justify-center">
          <div className="bg-white p-6 rounded-3xl shadow-2xl text-center">
            <img
              src="https://api.qrserver.com/v1/create-qr-code/?size=220x220&data=https://mastudio.com"
              alt="QR Code"
              className="rounded-2xl"
            />
            <p className="mt-4 font-semibold">Scan QR Code</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  {/* Domain & Hosting Guide */}
  <section className="max-w-6xl mx-auto px-6 pb-20">
    <div className="bg-white/10 rounded-3xl p-10 border border-white/10 shadow-2xl">
      <h2 className="text-4xl font-bold text-green-400 mb-8 text-center">
        Website Setup Guide
      </h2>

      <div className="grid md:grid-cols-3 gap-6">
        <div className="bg-slate-900 p-6 rounded-2xl">
          <h3 className="text-2xl font-bold mb-3">🌐 Domain</h3>
          <p className="text-slate-300">
            mastudio.com বা mastudiobd.com এর মতো নাম কিনতে হবে।
          </p>
        </div>

        <div className="bg-slate-900 p-6 rounded-2xl">
          <h3 className="text-2xl font-bold mb-3">☁️ Hosting</h3>
          <p className="text-slate-300">
            ওয়েবসাইট অনলাইনে চালু রাখতে হোস্টিং প্রয়োজন হবে।
          </p>
        </div>

        <div className="bg-slate-900 p-6 rounded-2xl">
          <h3 className="text-2xl font-bold mb-3">🚀 Publish</h3>
          <p className="text-slate-300">
            Domain ও Hosting যুক্ত করে ওয়েবসাইট লাইভ করা যাবে।
          </p>
        </div>
      </div>
    </div>
  </section>

<footer className="border-t border-white/10 py-6 text-center text-slate-400">
        © 2026 Ma Studio & Stationary | All Rights Reserved
      </footer>
    </div>
  );
}
