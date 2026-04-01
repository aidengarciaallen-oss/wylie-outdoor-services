# wylie-outdoor-servicesimport React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Phone, MapPin } from "lucide-react";
import Head from "next/head";

export default function HomePage() {
  return (
    <>
      {/* SEO Meta Tags */}
      <Head>
        <title>Wylie Lawn Care & Trash Can Cleaning | Landscaping Services in Wylie TX</title>
        <meta
          name="description"
          content="Affordable lawn care, trash can cleaning, and landscaping services in Wylie, Texas. Fast, reliable, and local. Get a free quote today!"
        />
        <meta name="keywords" content="Wylie Texas lawn care, trash can cleaning Wylie TX, landscaping Wylie TX, yard services near me" />
        <meta name="robots" content="index, follow" />

        {/* Open Graph (for social sharing) */}
        <meta property="og:title" content="Wylie Outdoor Services" />
        <meta property="og:description" content="Local lawn care, trash can cleaning, and landscaping in Wylie, TX." />
        <meta property="og:type" content="website" />

        {/* Local SEO Structured Data */}
        <script type="application/ld+json">
          {JSON.stringify({
            "@context": "https://schema.org",
            "@type": "LocalBusiness",
            name: "Wylie Outdoor Services",
            image: "https://via.placeholder.com/600x400",
            "@id": "",
            url: "https://yourwebsite.com",
            telephone: "+14690000000",
            address: {
              "@type": "PostalAddress",
              addressLocality: "Wylie",
              addressRegion: "TX",
              addressCountry: "US"
            },
            description:
              "Lawn care, trash can cleaning, and landscaping services in Wylie, Texas.",
            areaServed: "Wylie TX"
          })}
        </script>
      </Head>

      <div className="min-h-screen bg-gray-50 text-gray-900">
        {/* Header */}
        <header className="bg-green-700 text-white p-6 shadow-md">
          <h1 className="text-3xl font-bold">Wylie Outdoor Services</h1>
          <p className="text-sm">Lawn Care • Trash Can Cleaning • Landscaping</p>
        </header>

        {/* Hero Section */}
        <section className="text-center py-16 px-4 bg-green-100">
          <h2 className="text-4xl font-bold mb-4">Reliable Local Services in Wylie, TX</h2>
          <p className="mb-6 text-lg">Keeping your home clean, green, and looking great.</p>
          <Button className="text-lg px-6 py-3">Get a Free Quote</Button>
        </section>

        {/* Services */}
        <section className="py-12 px-6 grid md:grid-cols-3 gap-6">
          <Card className="rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-2">Lawn Care</h3>
              <p>Mowing, edging, trimming, and yard maintenance in Wylie, TX.</p>
            </CardContent>
          </Card>

          <Card className="rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-2">Trash Can Cleaning</h3>
              <p>Professional trash bin cleaning and sanitizing services in Wylie.</p>
            </CardContent>
          </Card>

          <Card className="rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-2">Landscaping</h3>
              <p>Custom landscaping, mulch, and yard upgrades in Wylie, Texas.</p>
            </CardContent>
          </Card>
        </section>

        {/* About */}
        <section className="bg-white py-12 px-6 text-center">
          <h2 className="text-2xl font-bold mb-4">Why Choose Us?</h2>
          <p className="max-w-xl mx-auto">
            We are a local Wylie-based business focused on quality work, fair pricing, and reliable service. Your satisfaction is our priority.
          </p>
        </section>

        {/* Contact */}
        <section className="bg-green-700 text-white py-12 px-6 text-center">
          <h2 className="text-2xl font-bold mb-4">Contact Us</h2>
          <div className="flex flex-col items-center gap-3">
            <p className="flex items-center gap-2"><Phone size={18}/> (469) 000-0000</p>
            <p className="flex items-center gap-2"><MapPin size={18}/> Wylie, Texas</p>
          </div>
          <Button className="mt-6 bg-white text-green-700 hover:bg-gray-200">Request Service</Button>
        </section>

        {/* Footer */}
        <footer className="text-center py-4 text-sm bg-gray-200">
          © {new Date().getFullYear()} Wylie Outdoor Services. All rights reserved.
        </footer>
      </div>
    </>
  );
}
