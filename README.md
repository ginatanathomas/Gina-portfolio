export default function GinaWebsite() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-neutral-100 to-stone-200 scroll-smooth">

      {/* NAVBAR */}
      <nav className="sticky top-0 bg-white shadow-md z-50">
        <div className="max-w-6xl mx-auto px-6 py-4 flex justify-between items-center">
          <h1 className="text-xl font-semibold tracking-wide">
            Gina Tana Thomas
          </h1>
          <div className="space-x-6 text-sm uppercase tracking-wider">
            <a href="#home" className="hover:text-gray-500">Home</a>
            <a href="#about" className="hover:text-gray-500">About</a>
            <a href="#portfolio" className="hover:text-gray-500">Portfolio</a>
            <a href="#contact" className="hover:text-gray-500">Contact</a>
          </div>
        </div>
      </nav>

      {/* HERO SECTION */}
      <section id="home" className="max-w-6xl mx-auto bg-white shadow-2xl rounded-2xl overflow-hidden grid md:grid-cols-2 mt-10">
        <div className="relative">
          <img
            src="/gina-photo.jpg"
            alt="Gina Tana Thomas"
            className="w-full h-full object-cover"
          />
          <div className="absolute inset-0 bg-black/20"></div>
        </div>

        <div className="p-12 flex flex-col justify-center">
          <h2 className="text-4xl font-light mb-4 tracking-wide">
            Luxury Interior Specialist
          </h2>

          <p className="text-gray-600 mb-6">
            Transforming spaces into timeless expressions of elegance,
            comfort, and emotional experience.
          </p>

          <a
            href="#contact"
            className="bg-black text-white px-6 py-3 rounded-2xl w-fit hover:opacity-90 transition"
          >
            Work With Me
          </a>
        </div>
      </section>

      {/* ABOUT */}
      <section id="about" className="max-w-5xl mx-auto mt-24 px-6">
        <div className="bg-white rounded-2xl shadow-xl p-12 text-center">
          <h2 className="text-3xl font-light mb-6 tracking-wide">
            About Me
          </h2>

          <p className="text-gray-700 leading-relaxed">
            I am a professional private contractor and interior decorator
            passionate about creating luxurious spaces that feel warm,
            intentional, and sophisticated. I combine structure,
            design precision, and emotional understanding to deliver
            refined results that stand the test of time.
          </p>
        </div>
      </section>

      {/* PORTFOLIO */}
      <section id="portfolio" className="max-w-6xl mx-auto mt-24 px-6">
        <h2 className="text-3xl font-light text-center mb-12 tracking-wide">
          My Work
        </h2>

        <div className="grid md:grid-cols-2 gap-10">
          <div className="bg-white shadow-xl rounded-2xl overflow-hidden">
            <img
              src="/interior-design-work.jpg"
              alt="Interior Planning"
              className="w-full h-80 object-cover"
            />
            <div className="p-6">
              <h3 className="text-xl font-medium mb-2">
                Concept & Design Planning
              </h3>
              <p className="text-gray-600">
                Careful selection of materials, textures, and tones
                to create harmony and elegance.
              </p>
            </div>
          </div>

          <div className="bg-white shadow-xl rounded-2xl overflow-hidden">
            <img
              src="/luxury-project-site.jpg"
              alt="Luxury Execution"
              className="w-full h-80 object-cover"
            />
            <div className="p-6">
              <h3 className="text-xl font-medium mb-2">
                Luxury Project Execution
              </h3>
              <p className="text-gray-600">
                Full supervision from structure to final details,
                ensuring premium quality and refined finishes.
              </p>
            </div>
          </div>
        </div>
      </section>

      {/* TESTIMONIALS */}
      <section className="max-w-5xl mx-auto mt-24 px-6">
        <div className="bg-neutral-900 text-white rounded-2xl shadow-2xl p-12">
          <h2 className="text-3xl font-light text-center mb-10 tracking-wide">
            Testimonials
          </h2>

          <div className="space-y-8">
            <p className="italic text-gray-300 text-center">
              “Professional, elegant, and deeply committed to excellence.
              The final result exceeded our expectations.”
            </p>

            <p className="italic text-gray-300 text-center">
              “A true luxury experience from start to finish.”
            </p>
          </div>
        </div>
      </section>

      {/* CONTACT */}
      <section id="contact" className="max-w-4xl mx-auto mt-24 mb-20 px-6">
        <div className="bg-white shadow-xl rounded-2xl p-12">
          <h2 className="text-3xl font-light text-center mb-8 tracking-wide">
            Contact Me
          </h2>

          <form className="space-y-6">
            <input
              type="text"
              placeholder="Your Name"
              className="w-full border p-3 rounded-xl focus:outline-none focus:ring-2 focus:ring-black"
            />

            <input
              type="email"
              placeholder="Your Email"
              className="w-full border p-3 rounded-xl focus:outline-none focus:ring-2 focus:ring-black"
            />

            <textarea
              placeholder="Your Message"
              rows="4"
              className="w-full border p-3 rounded-xl focus:outline-none focus:ring-2 focus:ring-black"
            ></textarea>

            <button
              type="submit"
              className="w-full bg-black text-white py-3 rounded-2xl hover:opacity-90 transition"
            >
              Send Message
            </button>
          </form>
        </div>
      </section>

      {/* FOOTER */}
      <footer className="bg-white border-t py-6 text-center text-sm text-gray-500">
        © {new Date().getFullYear()} Gina Tana Thomas. All rights reserved.
      </footer>

    </div>
  );
}
