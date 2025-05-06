import React from "react";
import { Mail, Linkedin } from "lucide-react";

export default function MiddlewareAdminPortfolio() {
  const skills = [
    "IBM WebSphere",
    "JBOSS / Wildfly",
    "Apache / Nginx / IHS",
    "AIX / Linux / Windows",
    "SSL/TLS Configuration",
    "Tivoli / Heap Analyzer",
    "Jenkins / GitHub",
    "Azure (AZ-900, AZ-204, AZ-400)",
    "Docker / Kubernetes",
  ];

  return (
    <div className="min-h-screen bg-gray-50 text-gray-800 font-sans">
      {/* Header */}
      <header className="bg-blue-800 text-white p-6 text-center shadow-md">
        <h1 className="text-4xl font-bold">Naveen C</h1>
        <p className="text-xl mt-2">Middleware System Administrator</p>
      </header>

      {/* About */}
      <section className="p-6 max-w-4xl mx-auto">
        <h2 className="text-2xl font-bold mb-2">About Me</h2>
        <p>
          As a dedicated Middleware Administrator with 2.5+ years of experience,
          I specialize in configuring, managing, and troubleshooting IBM WebSphere,
          Apache, Nginx, and JBOSS across AIX, Linux, and Windows environments.
          I'm Azure certified and passionate about cloud, DevOps, and IT infrastructure.
        </p>
      </section>

      {/* Skills */}
      <section className="p-6 bg-white">
        <h2 className="text-2xl font-bold mb-4 text-center">Technical Skills</h2>
        <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4 max-w-4xl mx-auto">
          {skills.map((skill, index) => (
            <div key={index} className="bg-blue-100 p-3 rounded shadow text-center">
              {skill}
            </div>
          ))}
        </div>
      </section>

      {/* Experience */}
      <section className="p-6 max-w-4xl mx-auto">
        <h2 className="text-2xl font-bold mb-4">Work Experience</h2>
        <div className="bg-gray-100 p-4 rounded shadow">
          <h3 className="text-xl font-semibold">TATA Consultancy Services</h3>
          <p className="text-sm text-gray-600">Middleware System Administrator | 2022 – Present</p>
          <ul className="list-disc list-inside mt-2 space-y-1">
            <li>Administered IBM WebSphere 8.5.5, including DMGR, clusters, and profiles</li>
            <li>Managed SSL, JDBC, J2C, Virtual Hosts, and plug-in propagation</li>
            <li>Deployed WAR/EAR applications and resolved production issues in real-time</li>
            <li>Provided 24/7 support, maintaining 99.9% uptime for healthcare clients</li>
          </ul>
        </div>
      </section>

      {/* Certifications */}
      <section className="p-6 bg-white max-w-4xl mx-auto">
        <h2 className="text-2xl font-bold mb-2">Certifications</h2>
        <ul className="list-disc list-inside space-y-1">
          <li>AZ-900: Microsoft Azure Fundamentals</li>
          <li>AZ-204: Developing Solutions for Microsoft Azure</li>
          <li>AZ-400: Microsoft DevOps Solutions</li>
          <li>DP-900: Azure Data Fundamentals</li>
          <li>DP-203: Data Engineering on Azure</li>
          <li>IBM WebSphere ND 8.5.5 Administration (Udemy)</li>
        </ul>
      </section>

      {/* Contact */}
      <section className="p-6 max-w-4xl mx-auto">
        <h2 className="text-2xl font-bold mb-2">Contact</h2>
        <p className="flex items-center gap-2"><Mail className="w-4 h-4" /> cnaveen014@gmail.com</p>
        <p className="flex items-center gap-2"><Linkedin className="w-4 h-4" /> <a href="https://www.linkedin.com/in/naveen-c-227075190" className="text-blue-600 underline">LinkedIn</a></p>
        <p>📍 Madipakkam, Chennai -91</p>
        <p>📞 +91 63820 55634</p>
      </section>

      {/* Footer */}
      <footer className="bg-blue-800 text-white text-center p-4 mt-6">
        © {new Date().getFullYear()} Naveen C — All Rights Reserved
      </footer>
    </div>
  );
}
