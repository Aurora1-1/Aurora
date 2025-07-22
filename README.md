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
    <div className={`min-h-screen ${darkMode ? 'bg-black text-white' : 'bg-gradient-to-b from-pink-800 via-purple-900 to-black text-white'} p-4 font-sans animate-fade-in-slow`}>
      <header className="flex flex-col items-center justify-center mb-6 animate-fade-in">
        <h1 className="text-5xl font-extrabold tracking-wide neon-text mb-2 animate-fade-in">Aurora</h1>
        <p className="italic text-lg neon-subtext mb-1 animate-slide-in">When Creativity Meets Intelligence</p>
        <p className="italic text-sm text-pink-300 mb-4 animate-slide-in">🚀 Launching on 1st February 2026</p>
        <div className="flex space-x-2">
          <button
            onClick={() => setDarkMode(!darkMode)}
            className="bg-pink-600 hover:bg-pink-800 text-white py-1 px-4 rounded-full shadow-lg hover:scale-105 transition-transform"
          >
            {darkMode ? 'Light Mode' : 'Dark Mode'}
          </button>
          <Link href="/create">
            <button className="bg-purple-600 hover:bg-purple-800 text-white py-1 px-4 rounded-full shadow-lg hover:scale-105 transition-transform">+ New Project</button>
          </Link>
        </div>
      </header>

      <section className="mb-8">
        <h2 className="text-2xl font-semibold mb-3 neon-subtext">Your Projects</h2>
        <div className="flex space-x-4 overflow-x-auto">
          {projects.map((project, idx) => (
            <div key={idx} className="bg-gradient-to-br from-pink-500 to-purple-700 text-white rounded-xl w-28 h-28 flex items-center justify-center shadow-xl transform hover:scale-110 transition-transform border-2 border-pink-300 animate-fade-in">
              {project}
            </div>
          ))}
        </div>
      </section>

      <section className="mb-10">
        <h2 className="text-2xl font-semibold mb-3 neon-subtext">Features</h2>
        <div className="grid grid-cols-2 md:grid-cols-3 gap-4">
          {features.map((feature, idx) => (
            <Link href={feature.route} key={idx}>
              <div className={`shadow-xl p-4 rounded-xl text-center cursor-pointer transform hover:scale-110 transition-transform border-2 border-pink-400 ${darkMode ? 'bg-gray-800 text-white' : 'bg-gray-900 text-white'} animate-slide-up`}>                <div className="text-4xl mb-2">⚡</div>
                <div className="font-bold neon-text">{feature.name}</div>
              </div>
            </Link>
          ))}
        </div>
      </section>

      <footer className={`fixed bottom-0 left-0 w-full border-t flex justify-around py-3 text-lg ${darkMode ? 'bg-gray-800 text-white' : 'bg-black text-pink-200'} shadow-inner animate-fade-in`}>
        <Link href="/edit">✂️ Edit</Link>
        <Link href="/templates">📋 Templates</Link>
        <Link href="/projects">🗂 Projects</Link>
        <Link href="/me">👤 Me</Link>
      </footer>

      <style jsx>{`
        .neon-text {
          color: #fff;
          text-shadow: 0 0 5px #fff, 0 0 10px #ff00ff, 0 0 20px #ff00ff;
        }
        .neon-subtext {
          color: #ddd;
          text-shadow: 0 0 3px #fff, 0 0 5px #ff00ff;
        }
        @keyframes fadeIn {
          from { opacity: 0; }
          to { opacity: 1; }
        }
        @keyframes slideIn {
          from { transform: translateY(20px); opacity: 0; }
          to { transform: translateY(0); opacity: 1; }
        }
        @keyframes slideUp {
          from { transform: translateY(50px); opacity: 0; }
          to { transform: translateY(0); opacity: 1; }
        }
        .animate-fade-in {
          animation: fadeIn 1s ease-in-out;
        }
        .animate-fade-in-slow {
          animation: fadeIn 2s ease-in-out;
        }
        .animate-slide-in {
          animation: slideIn 1s ease-out;
        }
        .animate-slide-up {
          animation: slideUp 1s ease-out;
        }
      `}</style>
    </div>
  );
}


