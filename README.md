# TELLINK_TELECOM
// pages/index.tsx
import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { BadgeCheck, Star } from "lucide-react";
import { motion } from "framer-motion";
import { Button } from "@/components/ui/button";
import { Carousel, CarouselContent, CarouselItem } from "@/components/ui/carousel";

const planos = [
  {
    titulo: "100 Mega",
    preco: "R$ 49,90",
    recursos: ["Wi-Fi 5 incluso"],
    observacao: "Consultar taxa de instalação"
  },
  {
    titulo: "150 Mega",
    preco: "R$ 59,90",
    recursos: ["Wi-Fi 5 incluso", "1ª parcela R$ 29,95", "50% de desconto na 1ª parcela"],
    observacao: "Consultar taxa de instalação"
  },
  {
    titulo: "300 Mega",
    preco: "R$ 69,90",
    recursos: ["Wi-Fi 5 incluso", "1ª parcela R$ 34,95", "50% de desconto na 1ª parcela"],
    observacao: "Consultar taxa de instalação",
    maisVendido: true
  },
  {
    titulo: "450 Mega",
    preco: "R$ 79,90",
    recursos: ["Wi-Fi 5 incluso", "1ª parcela R$ 39,95", "50% de desconto na 1ª parcela"],
    observacao: "Consultar taxa de instalação"
  },
  {
    titulo: "600 Mega",
    preco: "R$ 99,90",
    recursos: ["Wi-Fi 6 incluso", "4 parcelas de R$ 49,95", "50% de desconto nas 4 primeiras", "Suporte Premium"],
    observacao: "Consultar taxa de instalação"
  },
  {
    titulo: "1 Giga",
    preco: "R$ 199,90",
    recursos: ["Wi-Fi 6 incluso", "2 câmeras com IA ou alarme", "Suporte Premium"],
    observacao: "Consultar taxa de instalação"
  }
];

export default function HomePage() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-red-100 to-red-200">
      <header className="flex items-center justify-between px-6 py-4 bg-white shadow-md">
        <h1 className="text-2xl font-bold text-red-700">TELLINK TELECOM</h1>
        <nav className="space-x-6">
          <a href="#planos" className="text-gray-700 hover:text-red-600">Planos</a>
          <a href="#contato" className="text-gray-700 hover:text-red-600">Contato</a>
          <Button className="bg-green-600 hover:bg-green-700 text-white">Fale Conosco</Button>
        </nav>
      </header>

      <section className="text-center py-16 px-4 bg-red-600 text-white">
        <motion.h2 
          initial={{ opacity: 0, y: -20 }} 
          animate={{ opacity: 1, y: 0 }} 
          transition={{ duration: 0.5 }}
          className="text-4xl font-bold mb-4"
        >
          Conectando você ao futuro
        </motion.h2>
        <p className="text-lg mb-6">Internet de alta velocidade para sua casa ou empresa</p>
        <Button className="bg-white text-red-600 hover:bg-red-100">Assine pelo WhatsApp</Button>
      </section>

      <section id="planos" className="py-16 px-4 bg-white">
        <h3 className="text-3xl font-semibold text-center mb-10">Nossos Planos de Internet</h3>
        <Carousel>
          <CarouselContent>
            {planos.map((plano, index) => (
              <CarouselItem key={index} className="md:basis-1/3">
                <Card className="text-center p-6 bg-gray-50 shadow-md">
                  <CardContent>
                    <h4 className="text-2xl font-bold text-red-600 mb-2 flex justify-center items-center gap-2">
                      {plano.titulo}
                      {plano.maisVendido && <Star className="text-yellow-500" title="Mais contratado" />}
                    </h4>
                    <p className="text-xl font-semibold mb-4">{plano.preco}</p>
                    <ul className="mb-4 space-y-1 text-left text-sm">
                      {plano.recursos.map((recurso, i) => (
                        <li key={i} className="flex items-center gap-2">
                          <BadgeCheck className="text-green-500 w-4 h-4" />
                          {recurso}
                        </li>
                      ))}
                    </ul>
                    <p className="text-xs text-gray-500 italic">{plano.observacao}</p>
                  </CardContent>
                </Card>
              </CarouselItem>
            ))}
          </CarouselContent>
        </Carousel>
      </section>

      <section className="text-center py-10 px-4 bg-gray-100">
        <h3 className="text-2xl font-semibold mb-6">O que nossos clientes dizem</h3>
        <blockquote className="text-lg italic">“A Tellink superou minhas expectativas! A conexão é rápida e estável, recomendo a todos.”</blockquote>
        <p className="mt-2 font-semibold">— Lucas M.</p>
      </section>

      <footer className="bg-black text-white py-6 px-4 text-center space-y-2">
        <div className="space-x-4">
          <a href="#" className="hover:underline">Termos de Uso</a>
          <a href="#" className="hover:underline">Política de Privacidade</a>
        </div>
        <div className="flex justify-center gap-4 mt-2">
          <a href="#" aria-label="Facebook"><i className="fab fa-facebook"></i></a>
          <a href="#" aria-label="Instagram"><i className="fab fa-instagram"></i></a>
          <a href="#" aria-label="LinkedIn"><i className="fab fa-linkedin"></i></a>
        </div>
      </footer>
    </div>
  );
}
