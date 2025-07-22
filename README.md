import Link from 'next/link';
import { useState } from 'react';

export default function Home() {
  const features = [
    { name: 'AutoCut', route: '/features/autocut' },
    { name: 'Retouch', route: '/features/retouch' },
    { name: 'Space', route: '/features/space' },
    { name: 'Auto Enhance', route: '/features/auto-enhance' },
    { name: 'Photo Editor', route: '/features/photo-editor' },
    { name: 'Marketing Tools', route: '/features/marketing-tools' },
    { name: 'Remove Background', route: '/features/remove-background' },
    { name: 'Auto Captions', route: '/features/auto-captions' },
    { name: 'Camera', route: '/features/camera' }
  ];

  const [projects, setProjects] = useState([
    '20250721_1',
    '20250721_2',
    '2024_project',
    'Old Vibes'
  ]);

  const [darkMode, setDarkMode] = useState(false);

  return (
    <div className={`min-h-screen ${darkMode ? 'bg-gray-900 text-white' : 'bg-gradient-to-b from-blue-100 to-white text-black'} p-4 font-sans`}>
      <header className="flex items-center justify-between mb-6">
        <h1 className="text-3xl font-extrabold tracking-wide">Aurora</h1>
        <div className="flex space-x-2">
          <button
            onClick={() => setDarkMode(!darkMode)}
            className="bg-purple-500 hover:bg-purple-700 text-white py-1 px-3 rounded-full shadow"
          >
            {darkMode ? 'Light Mode' : 'Dark Mode'}
          </button>
          <Link href="/create">
            <button className="bg-blue-600 hover:bg-blue-800 text-white py-1 px-3 rounded-full shadow">+ New Project</button>
          </Link>
        </div>
      </header>

      <section className="mb-8">
        <h2 className="text-xl font-semibold mb-3">Your Projects</h2>
        <div className="flex space-x-4 overflow-x-auto">
          {projects.map((project, idx) => (
            <div key={idx} className="bg-gradient-to-br from-pink-400 to-purple-500 text-white rounded-xl w-28 h-28 flex items-center justify-center shadow-lg transform hover:scale-105 transition-transform">
              {project}
            </div>
          ))}
        </div>
      </section>

      <section className="mb-10">
        <h2 className="text-xl font-semibold mb-3">Features</h2>
        <div className="grid grid-cols-2 md:grid-cols-3 gap-4">
          {features.map((feature, idx) => (
            <Link href={feature.route} key={idx}>
              <div className={`shadow-lg p-4 rounded-xl text-center cursor-pointer transform hover:scale-105 transition-transform ${darkMode ? 'bg-gray-800 text-white' : 'bg-white text-gray-800'}`}>
                <div className="text-3xl mb-2">✨</div>
                <div className="font-medium">{feature.name}</div>
              </div>
            </Link>
          ))}
        </div>
      </section>

      <footer className={`fixed bottom-0 left-0 w-full border-t flex justify-around py-3 text-lg ${darkMode ? 'bg-gray-800 text-white' : 'bg-white text-black'} shadow-inner`}>
        <Link href="/edit">✂️ Edit</Link>
        <Link href="/templates">📋 Templates</Link>
        <Link href="/projects">🗂 Projects</Link>
        <Link href="/me">👤 Me</Link>
      </footer>
    </div>
  );
}

// Empty Feature Pages

export function AutoCut() {
  return <div className="p-10 text-center text-2xl">✨ AutoCut Feature Coming Soon!</div>;
}

export function Retouch() {
  return <div className="p-10 text-center text-2xl">✨ Retouch Feature Coming Soon!</div>;
}

export function Space() {
  return <div className="p-10 text-center text-2xl">✨ Space Feature Coming Soon!</div>;
}

export function AutoEnhance() {
  return <div className="p-10 text-center text-2xl">✨ Auto Enhance Feature Coming Soon!</div>;
}

export function PhotoEditor() {
  return <div className="p-10 text-center text-2xl">✨ Photo Editor Feature Coming Soon!</div>;
}

export function MarketingTools() {
  return <div className="p-10 text-center text-2xl">✨ Marketing Tools Feature Coming Soon!</div>;
}

export function RemoveBackground() {
  return <div className="p-10 text-center text-2xl">✨ Remove Background Feature Coming Soon!</div>;
}

export function AutoCaptions() {
  return <div className="p-10 text-center text-2xl">✨ Auto Captions Feature Coming Soon!</div>;
}

export function Camera() {
  return <div className="p-10 text-center text-2xl">✨ Camera Feature Coming Soon!</div>;
}
