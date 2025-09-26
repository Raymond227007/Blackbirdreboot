[index.html](https://github.com/user-attachments/files/22565970/index.html)
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Blackbirdbrowser Reboot</title>
    <link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Crect width='64' height='64' rx='12' fill='%235b21b6'/%3E%3Ctext x='50%' y='52%' dominant-baseline='middle' text-anchor='middle' font-size='24' font-family='Arial' fill='white'%3EBB%3C/text%3E%3C/svg%3E" />
    <!-- Tailwind CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- React 18 + ReactDOM UMD -->
    <script crossorigin src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
    <script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
    <!-- Babel for JSX (for this demo only) -->
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
  </head>
  <body class="bg-green-200 text-gray-900 antialiased">
    <div id="root"></div>

    <script type="text/babel">
      function Card({ title, desc }) {
        return (
          <div className="rounded-lg bg-white p-6 shadow-sm border">
            <div className="text-sm font-semibold">{title}</div>
            <div className="mt-3 text-sm text-gray-600">{desc}</div>
            <div className="mt-4">
              <a className="text-indigo-600 text-sm font-medium" href="#">Learn more →</a>
            </div>
          </div>
        );
      }

      function App() {
        return (
          <div className="min-h-screen">
            <header className="bg-white border-b">
              <div className="mx-auto max-w-7xl px-6 py-4 flex items-center justify-between">
                <div className="flex items-center gap-3">
                  <div className="h-10 w-10 rounded-lg bg-gradient-to-br from-indigo-600 to-purple-500 flex items-center justify-center text-white font-bold">BB</div>
                  <div>
                    <div className="font-semibold">Blackbird Browser</div>
                    <div className="text-xs text-gray-500">Reboot Edition</div>
                  </div>
                </div>

                <nav className="hidden md:flex items-center gap-6 text-sm">
                  <a className="hover:text-indigo-600" href="#mission">Mission</a>
                  <a className="hover:text-indigo-600" href="#features">Features</a>
                  <a className="hover:text-indigo-600" href="#community">Community</a>
                  <button className="ml-2 rounded-md bg-indigo-600 px-4 py-2 text-sm font-medium text-white hover:opacity-95">Download</button>
                </nav>

                <div className="md:hidden">
                  <button className="rounded-md border px-3 py-2">Menu</button>
                </div>
              </div>
            </header>

            <main className="mx-auto max-w-7xl px-6 py-12">
              <div className="grid grid-cols-1 md:grid-cols-2 gap-8 items-center">
                <div>
                  <h1 className="text-4xl font-extrabold leading-tight">The Browser Built With Us In Mind</h1>
                  <p className="mt-4 text-lg text-gray-700">Blackbird is back. A modern browser reboot created to empower Black and Brown communities online — with culture, identity, and connection at its core.</p>

                  <div className="mt-6 flex flex-wrap gap-3">
                    <a className="rounded-md bg-indigo-600 px-5 py-3 text-sm font-semibold text-white shadow" href="#">Join the movement</a>
                    <a className="rounded-md border px-5 py-3 text-sm font-medium" href="#community">Get involved</a>
                  </div>

                  <ul className="mt-8 grid grid-cols-1 sm:grid-cols-2 gap-3 text-sm text-gray-700">
                    <li>• Centering Black & Brown voices online</li>
                    <li>• A safe, private, and free browser</li>
                    <li>• Community-driven updates & features</li>
                    <li>• Merchandise: T‑shirts & hats coming soon</li>
                  </ul>
                </div>

                <div className="bg-white rounded-2xl p-6 shadow-md border text-center">
                  <div className="mb-4">
                    <div className="text-xs text-gray-500">Coming Soon</div>
                    <div className="mt-3 text-lg font-medium">Blackbird Reboot</div>
                  </div>
                  <p className="text-sm text-gray-600">Download the new version and show your support with community merch.</p>
                  <div className="mt-6 flex justify-center gap-3">
                    <button className="rounded-md bg-indigo-600 px-4 py-2 text-sm font-medium text-white">Download Free</button>
                    <button className="rounded-md border px-4 py-2 text-sm font-medium">Shop Merch</button>
                  </div>
                </div>
              </div>

              <section id="mission" className="mt-14">
                <h2 className="text-2xl font-semibold">Our Mission</h2>
                <p className="mt-2 text-gray-700 max-w-2xl">Blackbird was always more than a browser. It was a statement: that the internet should reflect the communities that use it. With this reboot, we aim to spark excitement, build pride, and create a platform where Black and Brown culture leads the experience.</p>
              </section>

              <section id="features" className="mt-14">
                <h2 className="text-2xl font-semibold">Features</h2>
                <div className="mt-6 grid grid-cols-1 md:grid-cols-3 gap-6">
                  <Card title="Community First" desc="Features and news curated for Black and Brown communities worldwide." />
                  <Card title="Privacy Built-In" desc="Ad-blocking and anti-tracking so your browsing stays safe." />
                  <Card title="Merch & Movement" desc="T‑shirts, hats, and events to spread the word and grow the movement." />
                </div>
              </section>

              <section id="community" className="mt-14 rounded-2xl bg-gradient-to-r from-indigo-600 to-purple-600 text-white p-8">
                <div className="max-w-4xl">
                  <h3 className="text-2xl font-semibold">Join the Community</h3>
                  <p className="mt-2">Blackbird Reboot is open-source, free, and powered by people. Be part of the movement to make browsing cultural, empowering, and ours.</p>

                  <div className="mt-6 flex gap-3">
                    <a href="mailto:info@blackbirdreboot.com" className="rounded-md bg-white/10 px-4 py-2 text-sm font-medium">Contact us</a>
                    <a href="#" className="rounded-md bg-white px-4 py-2 text-sm font-medium text-indigo-600">Contribute</a>
                  </div>
                </div>
              </section>
            </main>

            <footer className="mt-14 py-10 text-sm text-gray-600">
              <div className="max-w-7xl mx-auto flex flex-col md:flex-row items-center justify-between gap-6 px-6">
                <div>© {new Date().getFullYear()} Blackbirdbrowser Reboot</div>
                <div className="flex gap-6">
                  <a href="#">Privacy</a>
                  <a href="#">Terms</a>
                  <a href="mailto:info@blackbirdreboot.com">Contact</a>
                </div>
              </div>
            </footer>
          </div>
        );
      }

      const root = ReactDOM.createRoot(document.getElementById('root'));
      root.render(<App />);
    </script>
  </body>
</html>
