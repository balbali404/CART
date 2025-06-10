# CART

export const metadata: Metadata = {
  // 1. Primary SEO Meta Tags (Title, Description, Author)
  title: {
    default: 'Kunuze - Authentic Moroccan Traditional Clothing',
    template: '%s | Kunuze', // Dynamically append " | Kunuze" to page-specific titles
  },
  description: 'Kunuze is your premier online destination to sell exquisite Moroccan traditional clothes. Discover handcrafted caftans, djellabas, and accessories.',
  authors: [{ name: 'Balbali' }],
  creator: 'Balbali', // Could also be the company name if different from the author

  // 2. Canonical URL Setup
  // metadataBase is used to resolve relative URLs for other metadata fields.
  // It's best defined once in the root layout.
  metadataBase: new URL(METADATA_BASE_URL),
  alternates: {
    canonical: '/', // Default canonical for the homepage.
    // For specific pages, you would define this in their respective page.tsx
    // For example: canonical: '/products/caftan-royal'
  },

  // 3. Keywords (a comma-separated list of relevant terms)
  keywords: [
    'Moroccan traditional clothes',
    'Moroccan clothing',
    'Moroccan caftan',
    'Moroccan djellaba',
    'Moroccan gandoura',
    'Moroccan fashion',
    'Moroccan traditional dress',
    'Kunuze',
    'traditional wear',
    'handmade Moroccan clothing',
    'ethical fashion Morocco',
    'kaftan',
    'jellaba',
    'traditional Moroccan outfits',
    'North African fashion',
    'ethnic wear',
    'artisanal clothing',
    'Moroccan style',
    'online store Moroccan clothes',
    'buy caftan online',
    'morocco shop'
  ],

  // 4. Open Graph Meta Tags (for social media sharing like Facebook, LinkedIn)
  openGraph: {
    title: 'Kunuze - Authentic Moroccan Traditional Clothing',
    description: 'Kunuze is your premier online destination to sell exquisite Moroccan traditional clothes. Discover handcrafted caftans, djellabas, and accessories.',
    url: METADATA_BASE_URL,
    siteName: 'Kunuze',
    images: [
      {
        url: `${METADATA_BASE_URL}/images/og-image-kunuze.jpg`, // IMPORTANT: Replace with your actual OG image URL (1200x630px recommended)
        width: 1200,
        height: 630,
        alt: 'Kunuze Moroccan Traditional Clothing - Social Share Image',
      },
      // You can add more image sizes or types here if needed
    ],
    locale: 'en_US', // Or 'fr_FR' if your primary content is French
    type: 'website', // Use 'website' for homepage, 'product' for product pages, 'article' for blog posts
  },

  // 5. Twitter Card Meta Tags (for Twitter/X sharing)
  twitter: {
    card: 'summary_large_image', // Use 'summary_large_image' for a prominent image
    title: 'Kunuze - Authentic Moroccan Traditional Clothing',
    description: 'Discover handcrafted Moroccan caftans, djellabas, and accessories at Kunuze. Your premier online store for traditional Moroccan wear.',
    site: '@KunuzeOfficial', // IMPORTANT: Replace with your actual Twitter handle
    creator: '@BalbaliOfficial', // IMPORTANT: Replace with the author's Twitter handle if applicable
    images: {
      url: `${METADATA_BASE_URL}/images/twitter-image-kunuze.jpg`, // IMPORTANT: Replace with your actual Twitter image URL (800x418px recommended)
      alt: 'Kunuze Moroccan Traditional Clothing - Twitter Image',
    },
  },

  // 6. Viewport and Charset (Next.js handles these by default, but you can explicitly define if needed)
  // viewport: {
  //   width: 'device-width',
  //   initialScale: 1,
  //   maximumScale: 1,
  // },
  // charset: 'utf-8', // This is generally handled automatically by Next.js/React
};
