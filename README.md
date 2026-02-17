# Pib
Pib

Action: file_editor create /app/frontend/src/App.js --file-text "import React from \"react\";
import { BrowserRouter, Routes, Route } from \"react-router-dom\";
import { Toaster } from \"./components/ui/sonner\";
import Header from \"./components/Header\";
import Footer from \"./components/Footer\";
import Home from \"./pages/Home\";
import Doutrinas from \"./pages/Doutrinas\";
import Horarios from \"./pages/Horarios\";
import Batismo from \"./pages/Batismo\";
import EBD from \"./pages/EBD\";
import Pastores from \"./pages/Pastores\";
import Embaixadores from \"./pages/Embaixadores\";
import Pescadores from \"./pages/Pescadores\";
import Contato from \"./pages/Contato\";
import \"./App.css\";

function App() {
  return (
    <BrowserRouter>
      <div className=\"flex flex-col min-h-screen\">
        <Header />
        <main className=\"flex-grow\">
          <Routes>
            <Route path=\"/\" element={<Home />} />
            <Route path=\"/doutrinas\" element={<Doutrinas />} />
            <Route path=\"/horarios\" element={<Horarios />} />
            <Route path=\"/batismo\" element={<Batismo />} />
            <Route path=\"/ebd\" element={<EBD />} />
            <Route path=\"/pastores\" element={<Pastores />} />
            <Route path=\"/embaixadores\" element={<Embaixadores />} />
            <Route path=\"/pescadores\" element={<Pescadores />} />
            <Route path=\"/contato\" element={<Contato />} />
          </Routes>
        </main>
        <Footer />
        <Toaster position=\"top-right\" />
      </div>
    </BrowserRouter>
  );
}

export default App;
"
Observation: Overwrite successful: /app/frontend/src/App.js
