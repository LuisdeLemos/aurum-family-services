import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";

export default function Home() {
  return (
    <div className="min-h-screen bg-gray-100">
      {/* Header */}
      <header className="bg-white shadow p-4 flex justify-between items-center">
        <h1 className="text-2xl font-bold text-gray-800">Aurum Family Services</h1>
        <Button className="bg-gold-500 text-white">Contacto</Button>
      </header>

      {/* Hero Section */}
      <section className="flex flex-col items-center justify-center text-center py-20 bg-[url('/hero.jpg')] bg-cover bg-center">
        <h2 className="text-4xl font-bold text-white">Servicios Exclusivos para Familias Extranjeras</h2>
        <p className="text-white mt-4 max-w-xl">
          Asesoramiento en educación, lifestyle, hogar y gestión patrimonial en España.
        </p>
        <Button className="mt-6 bg-gold-500 text-white">Descubre más</Button>
      </section>

      {/* Servicios */}
      <section className="py-16 px-4">
        <h2 className="text-3xl font-bold text-center text-gray-800 mb-8">Nuestros Servicios</h2>
        <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
          <Card>
            <CardContent className="p-4">
              <h3 className="text-xl font-semibold">Asesoramiento Educativo</h3>
              <p className="text-gray-600">Universidades, colegios y clubs exclusivos.</p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-4">
              <h3 className="text-xl font-semibold">Lifestyle & Concierge</h3>
              <p className="text-gray-600">Reservas en restaurantes y eventos VIP.</p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-4">
              <h3 className="text-xl font-semibold">Hogar y Diseño</h3>
              <p className="text-gray-600">Reformas, decoración y mantenimiento.</p>
            </CardContent>
          </Card>
        </div>
      </section>

      {/* Contacto */}
      <section className="py-16 bg-gray-200 text-center">
        <h2 className="text-3xl font-bold text-gray-800">Contáctanos</h2>
        <p className="text-gray-600 mt-2">Déjanos tu mensaje y te responderemos pronto.</p>
        <form className="mt-6 max-w-lg mx-auto">
          <input type="text" placeholder="Tu nombre" className="w-full p-3 border rounded mb-4" />
          <input type="email" placeholder="Tu correo" className="w-full p-3 border rounded mb-4" />
          <textarea placeholder="Tu mensaje" className="w-full p-3 border rounded mb-4"></textarea>
          <Button className="bg-gold-500 text-white w-full">Enviar</Button>
        </form>
      </section>
    </div>
  );
}
