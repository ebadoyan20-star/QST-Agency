import React from "react";
import { motion } from "framer-motion";

// Single-file React component: DigitasLikeLanding
// Tailwind CSS classes assumed to be available in the project.
// This component is a starting point — hero, services, case studies, contact CTA, footer.
// Default export a React component so it can be dropped into a Next.js / CRA page.

export default function DigitasLikeLanding() {
  return (
    <div className="min-h-screen bg-white text-slate-800 antialiased">
      {/* Navbar */}
      <header className="w-full border-b border-slate-100">
        <div className="max-w-7xl mx-auto px-6 py-5 flex items-center justify-between">
          <div className="flex items-center gap-4">
            <div className="w-10 h-10 bg-gradient-to-r from-indigo-600 to-teal-400 rounded-lg flex items-center justify-center text-white font-bold">Q</div>
            <div>
              <span className="font-semibold text-lg">QST Agency</span>
              <div className="text-xs text-slate-500">Strategic Digital Experiences</div>
            </div>
          </div>

          <nav className="hidden md:flex items-center gap-6 text-sm text-slate-600">
            <a href="#work" className="hover:text-slate-900">Work</a>
            <a href="#services" className="hover:text-slate-900">Services</a>
            <a href="#insights" className="hover:text-slate-900">Insights</a>
            <a href="#careers" className="hover:text-slate-900">Careers</a>
            <a href="#contact" className="px-4 py-2 bg-slate-900 text-white rounded-md">Contact</a>
          </nav>

          <button className="md:hidden p-2 rounded-md border border-slate-200">Menu</button>
        </div>
      </header>

      {/* Hero */}
      <main>
        <section className="bg-gradient-to-b from-slate-50 to-white">
          <div className="max-w-7xl mx-auto px-6 py-20 grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
            <div>
              <motion.h1
                initial={{ opacity: 0, y: 10 }}
                animate={{ opacity: 1, y: 0 }}
                transition={{ duration: 0.6 }}
                className="text-4xl md:text-5xl font-extrabold leading-tight"
              >
                Creative strategy. Built for measurable growth.
              </motion.h1>

              <motion.p
                initial={{ opacity: 0 }}
                animate={{ opacity: 1 }}
                transition={{ delay: 0.2, duration: 0.6 }}
                className="mt-6 text-lg text-slate-600 max-w-xl"
              >
                We design integrated digital experiences — from awareness to conversion — for ambitious brands.
                Our work blends human insight, creative excellence and data-driven media.
              </motion.p>

              <div className="mt-8 flex gap-4">
                <a href="#contact" className="inline-flex items-center gap-3 px-5 py-3 bg-slate-900 text-white rounded-md font-medium">Start a project</a>
                <a href="#work" className="inline-flex items-center gap-3 px-5 py-3 border border-slate-200 rounded-md text-slate-700">See our work</a>
              </div>

              <div className="mt-8 text-sm text-slate-500">
                <strong>Industries:</strong> Retail · Finance · Healthcare · Manufacturing
              </div>
            </div>

            <div className="order-first md:order-last">
              <div className="relative">
                <div className="bg-gradient-to-br from-indigo-100 to-teal-50 p-6 rounded-2xl shadow-lg">
                  <img
                    src="https://images.unsplash.com/photo-1542744173-8e7e53415bb0?q=80&w=1400&auto=format&fit=crop"
                    alt="Campaign preview"
                    className="w-full rounded-lg object-cover h-72"
                  />
                </div>
                <div className="absolute -bottom-6 left-6 bg-white border border-slate-100 rounded-lg p-4 shadow-md w-64">
                  <div className="text-xs text-slate-500">Latest campaign</div>
                  <div className="font-semibold">Furniture brand launch — +42% conversion</div>
                </div>
              </div>
            </div>
          </div>
        </section>

        {/* Services */}
        <section id="services" className="max-w-7xl mx-auto px-6 py-20">
          <div className="text-center">
            <div className="text-sm text-teal-600 font-medium">What we do</div>
            <h2 className="text-3xl font-bold mt-2">Integrated services — strategy to activation</h2>
            <p className="mt-3 text-slate-600 max-w-2xl mx-auto">Brand strategy, creative, content, UX, media buying and analytics — combined to drive measurable business outcomes.</p>
          </div>

          <div className="mt-12 grid grid-cols-1 md:grid-cols-3 gap-8">
            {[
              { title: 'Brand & Strategy', desc: 'Positioning, research, experience strategy.' },
              { title: 'Creative & Design', desc: 'Campaign creative, visual systems, motion.' },
              { title: 'Media & Performance', desc: 'Paid social, search, programmatic, measurement.' },
            ].map((s) => (
              <motion.div key={s.title} whileHover={{ y: -6 }} className="p-6 border border-slate-100 rounded-xl bg-white">
                <div className="text-sm text-teal-600 font-semibold">{s.title}</div>
                <div className="mt-3 text-slate-700">{s.desc}</div>
                <div className="mt-4 text-sm text-slate-500">From CAD $2,500/month</div>
              </motion.div>
            ))}
          </div>
        </section>

        {/* Case studies / Work gallery */}
        <section id="work" className="bg-slate-50 py-20">
          <div className="max-w-7xl mx-auto px-6">
            <div className="flex items-center justify-between">
              <div>
                <h3 className="text-2xl font-bold">Selected work</h3>
                <p className="mt-2 text-slate-600">Award-winning integrated campaigns with measurable ROI.</p>
              </div>
              <a href="#work" className="text-sm text-slate-700">View all case studies →</a>
            </div>

            <div className="mt-8 grid grid-cols-1 md:grid-cols-3 gap-6">
              {[1, 2, 3].map((i) => (
                <article key={i} className="rounded-lg overflow-hidden shadow-sm bg-white">
                  <img src={https://images.unsplash.com/photo-1504384308090-c894fdcc538d?q=80&w=1400&auto=format&fit=crop} alt={case ${i}} className="h-48 w-full object-cover" />
                  <div className="p-5">
                    <div className="text-xs text-teal-600 font-medium">Retail</div>
                    <h4 className="mt-2 font-semibold">Campaign Title {i}</h4>
                    <p className="mt-2 text-sm text-slate-600">Short blurb about the challenge and results — +30% traffic, +18% revenue.</p>
                    <div className="mt-4">
                      <a className="text-sm text-slate-700">Read case study →</a>
                    </div>
                  </div>
                </article>
              ))}
            </div>
          </div>
        </section>

        {/* Insights / Blog */}
        <section id="insights" className="max-w-7xl mx-auto px-6 py-20">
          <div className="text-center">
            <h3 className="text-2xl font-bold">Insights</h3>
            <p className="mt-2 text-slate-600">Thought leadership on creativity, media and technology.</p>
          </div>

          <div className="mt-8 grid grid-cols-1 md:grid-cols-3 gap-6">
            {[1, 2, 3].map((i) => (
              <div key={i} className="p-6 border border-slate-100 rounded-xl">
                <div className="text-xs text-slate-500">Oct {10 + i}, 2025</div>
                <h4 className="mt-2 font-semibold">Article title {i}</h4>
                <p className="mt-2 text-sm text-slate-600">Brief summary of an article about media trends and measurement.</p>
                <div className="mt-4 text-sm text-teal-600">Read →</div>
              </div>
            ))}
          </div>
        </section>

        {/* Contact CTA */}
        <section id="contact" className="bg-gradient-to-r from-indigo-600 to-teal-500 text-white py-16">
          <div className="max-w-4xl mx-auto px-6 text-center">
            <h3 className="text-3xl font-bold">Let’s build something together</h3>
            <p className="mt-3">Tell us about your challenge and we’ll propose an approach tailored to your goals.</p>

            <div className="mt-8 flex flex-col sm:flex-row justify-center gap-4">
              <a href="mailto:hello@qstagency.com" className="px-6 py-3 bg-white text-indigo-700 rounded-md font-medium inline-block">Email us</a>
              <a href="#" className="px-6 py-3 border border-white rounded-md inline-block">Request proposal</a>
            </div>
          </div>
        </section>

        {/* Footer */}
        <footer className="border-t border-slate-100">
          <div className="max-w-7xl mx-auto px-6 py-10 grid grid-cols-1 md:grid-cols-3 gap-6">
            <div>
              <div className="font-semibold">QST Agency</div>
              <div className="mt-2 text-sm text-slate-500">Strategic digital experiences — Vancouver & remote.</div>
            </div>

            <div className="flex gap-8">
              <div>
                <div className="font-semibold">Services</div>
                <ul className="mt-2 text-sm text-slate-600">
                  <li>Brand & Strategy</li>
                  <li>Creative</li>
                  <li>Media</li>
                </ul>
              </div>

              <div>
                <div className="font-semibold">Contact</div>
                <div className="mt-2 text-sm text-slate-600">hello@qstagency.com</div>
                <div className="text-sm text-slate-600">+1 (604) 555-0123</div>
              </div>
            </div>

            <div className="text-sm text-slate-500">© {new Date().getFullYear()} QST Agency. All rights reserved.</div>
          </div>
        </footer>
      </main>
    </div>
  );
}
