import { useContext } from 'react';
import { Link } from 'react-router-dom';
import { DataContext } from '../providers/DataProvider';
import { about } from '../content/about';
import Navbar from '../components/Navbar';

const About = () => {
  const appContext = useContext(DataContext);
  if (!appContext) return null;
  const { lang, setLang } = appContext;

  return (
    <div className="min-h-screen flex flex-col md:max-w-xl lg:max-w-6xl mx-auto">
      <Navbar />
      <main className="my-auto p-6">
        <h1 className="font-semibold text-3xl lg:text-[40px] text-zinc-800 mt-6 whitespace-pre-wrap mb-12">
          {about.header[lang]}
        </h1>
        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
          {about.subheader[lang]}
        </div>
        
      </main>
    </div>
  );
};

export default About;
