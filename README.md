import React from "react";
s
export default function App() {
  return (
    <main className="bg-gradient-to-b from-slate-100 to-white min-h-screen font-sans">
      {/* Encabezado */}
      <header className="bg-white shadow-lg py-10 px-4 text-center border-b border-gray-200">
        <h1 className="text-4xl font-extrabold text-slate-800 tracking-tight">Facundo - Desarrollador React Native</h1>
        <p className="text-slate-500 mt-3 text-lg">Apasionado por la tecnología y el desarrollo de apps móviles</p>
      </header>

      {/* Sección Sobre mí */}
      <section className="px-6 py-12 max-w-5xl mx-auto">
        <h2 className="text-3xl font-bold text-slate-800 mb-6 border-b pb-2 border-blue-200">Sobre mí</h2>
        <p className="text-slate-600 text-lg leading-relaxed">
          Soy un desarrollador con experiencia en aplicaciones móviles usando React Native, Firebase y herramientas modernas. Me enfoco en construir interfaces intuitivas y soluciones funcionales para el usuario final.
        </p>
      </section>

      {/* Sección Proyectos */}
      <section className="bg-white p-10 max-w-5xl mx-auto rounded-lg shadow-md mb-12">
        <h2 className="text-3xl font-bold text-slate-800 mb-6 border-b pb-2 border-blue-200">Proyectos</h2>
        <div className="grid gap-6 md:grid-cols-2">
          <div className="bg-slate-50 p-6 rounded-lg shadow hover:shadow-lg transition-shadow">
            <h3 className="text-xl font-semibold text-blue-600">App de Gestión de Tolvas</h3>
            <p className="text-slate-600 mt-2">App móvil para controlar motores de carga y descarga, desarrollada en React Native y Firebase.</p>
            <a
              href="https://github.com/facundo/tolvas-app"
              target="_blank"
              rel="noopener noreferrer"
              className="inline-block mt-4 text-blue-500 hover:underline"
            >
              Ver en GitHub
            </a>
          </div>
        </div>
      </section>

      {/* Sección Tecnologías */}
      <section className="px-6 pb-12 max-w-5xl mx-auto">
        <h2 className="text-3xl font-bold text-slate-800 mb-6 border-b pb-2 border-blue-200">Tecnologías</h2>
        <div className="flex flex-wrap gap-4">
          {['React Native', 'Firebase', 'JavaScript', 'Tailwind CSS', 'Git'].map((tech) => (
            <span key={tech} className="bg-blue-100 text-blue-800 px-3 py-1 rounded-full text-sm font-medium">
              {tech}
            </span>
          ))}
        </div>
      </section>

      {/* Contacto */}
      <footer className="bg-slate-100 py-8 text-center border-t border-gray-300">
        <h2 className="text-2xl font-semibold text-slate-700">Contacto</h2>
        <p className="mt-2 text-slate-600">
          <a href="mailto:facundo@email.com" className="text-blue-600 hover:underline">facundo@email.com</a>
        </p>
        <p className="mt-2 text-slate-600">
          <a href="https://github.com/facundo" target="_blank" rel="noopener noreferrer" className="text-blue-600 hover:underline">Mi GitHub</a>
        </p>
      </footer>
    </main>
  );
}
