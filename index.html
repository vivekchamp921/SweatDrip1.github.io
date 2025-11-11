import React, { useState, useEffect } from 'react';
import { Menu, X, ShoppingBag, Heart, Search, Star, ChevronRight, ArrowRight, Check, Minus, Plus } from 'lucide-react';

interface Product {
  id: number;
  name: string;
  category: string;
  price: number;
  rating: number;
  image: string;
  isNew?: boolean;
  isBestseller?: boolean;
}

interface CartItem extends Product {
  size: string;
  quantity: number;
}

export default function FitnessBrand() {
  const [mobileMenuOpen, setMobileMenuOpen] = useState(false);
  const [selectedCategory, setSelectedCategory] = useState('all');
  const [cartOpen, setCartOpen] = useState(false);
  const [cart, setCart] = useState<CartItem[]>([]);
  const [selectedProduct, setSelectedProduct] = useState<Product | null>(null);
  const [selectedSize, setSelectedSize] = useState('');
  const [email, setEmail] = useState('');
  const [scrolled, setScrolled] = useState(false);

  useEffect(() => {
    const handleScroll = () => {
      setScrolled(window.scrollY > 20);
    };
    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  }, []);

  const products: Product[] = [
    { 
      id: 1, 
      name: 'Performance Tank Pro', 
      category: 'women', 
      price: 68, 
      rating: 4.8, 
      image: 'https://images.unsplash.com/photo-1567401893414-76b7b1e5a7a5?w=800&h=800&fit=crop',
      isNew: true 
    },
    { 
      id: 2, 
      name: 'Elite Training Shorts', 
      category: 'men', 
      price: 85, 
      rating: 4.9, 
      image: 'https://images.unsplash.com/photo-1556906781-9a412961c28c?w=800&h=800&fit=crop',
      isBestseller: true 
    },
    { 
      id: 3, 
      name: 'Flex Leggings', 
      category: 'women', 
      price: 95, 
      rating: 4.7,
      image: 'https://images.unsplash.com/photo-1506629082955-511b1aa562c8?w=800&h=800&fit=crop'
    },
    { 
      id: 4, 
      name: 'Power Hoodie', 
      category: 'men', 
      price: 120, 
      rating: 4.6,
      image: 'https://images.unsplash.com/photo-1614495039153-e9cd13240469?w=800&h=800&fit=crop'
    },
    { 
      id: 5, 
      name: 'Studio Sports Bra', 
      category: 'women', 
      price: 58, 
      rating: 4.9,
      image: 'https://images.unsplash.com/photo-1594381898411-846e7d193883?w=800&h=800&fit=crop',
      isBestseller: true 
    },
    { 
      id: 6, 
      name: 'Velocity Running Tee', 
      category: 'men', 
      price: 75, 
      rating: 4.5,
      image: 'https://images.unsplash.com/photo-1523381294911-8d3cead13475?w=800&h=800&fit=crop',
      isNew: true 
    },
  ];

  const filteredProducts = selectedCategory === 'all' 
    ? products 
    : products.filter(p => p.category === selectedCategory);

  const addToCart = (product: Product) => {
    if (!selectedSize) return;
    
    const existingItem = cart.find(item => item.id === product.id && item.size === selectedSize);
    
    if (existingItem) {
      setCart(cart.map(item => 
        item.id === product.id && item.size === selectedSize 
          ? { ...item, quantity: item.quantity + 1 }
          : item
      ));
    } else {
      setCart([...cart, { ...product, size: selectedSize, quantity: 1 }]);
    }
    
    setSelectedProduct(null);
    setSelectedSize('');
    setCartOpen(true);
  };

  const updateQuantity = (id: number, size: string, delta: number) => {
    setCart(cart.map(item => {
      if (item.id === id && item.size === size) {
        const newQuantity = item.quantity + delta;
        return newQuantity > 0 ? { ...item, quantity: newQuantity } : null;
      }
      return item;
    }).filter(Boolean) as CartItem[]);
  };

  const cartTotal = cart.reduce((sum, item) => sum + (item.price * item.quantity), 0);
  const cartCount = cart.reduce((sum, item) => sum + item.quantity, 0);

  return (
    <div className="min-h-screen bg-white">
      {/* Header */}
      <header className={`fixed top-0 w-full z-50 transition-all duration-300 ${scrolled ? 'bg-white shadow-lg' : 'bg-transparent'}`}>
        <div className="container mx-auto px-4">
          <div className="flex items-center justify-between h-20">
            <div className="flex items-center space-x-8">
              <h1 className={`text-2xl font-black tracking-tight ${scrolled ? 'text-gray-900' : 'text-white'}`}>
                Sweat<span className="text-red-500">Drip</span>
              </h1>
              <nav className="hidden md:flex space-x-6">
                {['New Arrivals', 'Women', 'Men', 'Collections', 'Sale'].map((item) => (
                  <button
                    key={item}
                    className={`font-medium transition-colors hover:text-red-500 ${scrolled ? 'text-gray-700' : 'text-white'}`}
                  >
                    {item}
                  </button>
                ))}
              </nav>
            </div>
            
            <div className="flex items-center space-x-4">
              <button className={`p-2 rounded-full hover:bg-gray-100 transition-colors ${scrolled ? 'text-gray-700' : 'text-white'}`}>
                <Search className="w-5 h-5" />
              </button>
              <button className={`p-2 rounded-full hover:bg-gray-100 transition-colors ${scrolled ? 'text-gray-700' : 'text-white'}`}>
                <Heart className="w-5 h-5" />
              </button>
              <button 
                onClick={() => setCartOpen(true)}
                className={`p-2 rounded-full hover:bg-gray-100 transition-colors relative ${scrolled ? 'text-gray-700' : 'text-white'}`}
              >
                <ShoppingBag className="w-5 h-5" />
                {cartCount > 0 && (
                  <span className="absolute -top-1 -right-1 bg-red-500 text-white text-xs rounded-full w-5 h-5 flex items-center justify-center">
                    {cartCount}
                  </span>
                )}
              </button>
              <button 
                onClick={() => setMobileMenuOpen(!mobileMenuOpen)}
                className={`md:hidden p-2 ${scrolled ? 'text-gray-700' : 'text-white'}`}
              >
                {mobileMenuOpen ? <X className="w-6 h-6" /> : <Menu className="w-6 h-6" />}
              </button>
            </div>
          </div>
        </div>
      </header>

      {/* Hero Section */}
      <section className="relative h-screen flex items-center justify-center overflow-hidden">
        <div 
          className="absolute inset-0 bg-cover bg-center"
          style={{
            backgroundImage: 'url(https://images.unsplash.com/photo-1534438327276-14e5300c3a48?w=1920&h=1080&fit=crop)'
          }}
        />
        <div className="absolute inset-0 bg-gradient-to-br from-black via-gray-900 to-transparent opacity-70" />
        
        <div className="relative z-10 text-center text-white px-4 max-w-4xl mx-auto">
          <p className="text-red-500 font-bold tracking-widest mb-4">UNLEASH YOUR POTENTIAL</p>
          <h2 className="text-5xl md:text-7xl font-black mb-6 leading-tight">
            TRAIN HARDER.<br />LOOK BETTER.
          </h2>
          <p className="text-xl mb-8 text-gray-300 max-w-2xl mx-auto">
            Premium activewear engineered for peak performance and unmatched style. 
            Elevate your fitness journey with gear that moves with you.
          </p>
          <div className="flex flex-col sm:flex-row gap-4 justify-center">
            <button className="bg-red-500 text-white px-8 py-4 font-bold hover:bg-red-600 transition-all transform hover:scale-105">
              SHOP WOMEN
            </button>
            <button className="bg-white text-gray-900 px-8 py-4 font-bold hover:bg-gray-100 transition-all transform hover:scale-105">
              SHOP MEN
            </button>
          </div>
        </div>
        
        <div className="absolute bottom-8 left-1/2 transform -translate-x-1/2 animate-bounce">
          <ChevronRight className="w-6 h-6 text-white rotate-90" />
        </div>
      </section>

      {/* Lifestyle Banner */}
      <section className="py-16 bg-black">
        <div className="container mx-auto px-4">
          <div className="grid md:grid-cols-2 gap-8">
            <div 
              className="relative h-96 bg-cover bg-center rounded-lg overflow-hidden group cursor-pointer"
              style={{
                backgroundImage: 'url(https://images.unsplash.com/photo-1518611012118-696072aa579a?w=800&h=600&fit=crop)'
              }}
            >
              <div className="absolute inset-0 bg-gradient-to-t from-black via-transparent to-transparent opacity-60" />
              <div className="absolute bottom-8 left-8 text-white">
                <h3 className="text-3xl font-black mb-2">WOMEN'S COLLECTION</h3>
                <p className="mb-4">Engineered for strength & style</p>
                <button className="bg-white text-black px-6 py-2 font-bold hover:bg-gray-100 transition-all">
                  EXPLORE NOW
                </button>
              </div>
            </div>
            <div 
              className="relative h-96 bg-cover bg-center rounded-lg overflow-hidden group cursor-pointer"
              style={{
                backgroundImage: 'url(https://images.unsplash.com/photo-1605296867424-35fc25c9212a?w=800&h=600&fit=crop)'
              }}
            >
              <div className="absolute inset-0 bg-gradient-to-t from-black via-transparent to-transparent opacity-60" />
              <div className="absolute bottom-8 left-8 text-white">
                <h3 className="text-3xl font-black mb-2">MEN'S COLLECTION</h3>
                <p className="mb-4">Built for champions</p>
                <button className="bg-white text-black px-6 py-2 font-bold hover:bg-gray-100 transition-all">
                  EXPLORE NOW
                </button>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Category Tabs */}
      <section className="py-16 bg-gray-50">
        <div className="container mx-auto px-4">
          <div className="text-center mb-12">
            <h3 className="text-4xl font-black mb-4">FEATURED COLLECTION</h3>
            <p className="text-gray-600">Discover our most popular performance gear</p>
          </div>
          
          <div className="flex justify-center mb-8">
            <div className="inline-flex bg-white rounded-full shadow-md p-1">
              {['all', 'women', 'men'].map((category) => (
                <button
                  key={category}
                  onClick={() => setSelectedCategory(category)}
                  className={`px-6 py-2 rounded-full font-medium transition-all ${
                    selectedCategory === category
                      ? 'bg-gray-900 text-white'
                      : 'text-gray-600 hover:text-gray-900'
                  }`}
                >
                  {category.charAt(0).toUpperCase() + category.slice(1)}
                </button>
              ))}
            </div>
          </div>

          {/* Product Grid */}
          <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            {filteredProducts.map((product) => (
              <div key={product.id} className="group cursor-pointer" onClick={() => setSelectedProduct(product)}>
                <div className="relative overflow-hidden bg-gray-200 aspect-square mb-4">
                  <img 
                    src={product.image} 
                    alt={product.name}
                    className="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500"
                  />
                  {product.isNew && (
                    <span className="absolute top-4 left-4 bg-red-500 text-white px-3 py-1 text-xs font-bold">NEW</span>
                  )}
                  {product.isBestseller && (
                    <span className="absolute top-4 left-4 bg-gray-900 text-white px-3 py-1 text-xs font-bold">BESTSELLER</span>
                  )}
                  <div className="absolute inset-0 bg-black opacity-0 group-hover:opacity-20 transition-opacity" />
                  <button className="absolute bottom-4 left-1/2 transform -translate-x-1/2 bg-white text-gray-900 px-6 py-2 font-bold opacity-0 group-hover:opacity-100 transition-all translate-y-2 group-hover:translate-y-0">
                    QUICK VIEW
                  </button>
                </div>
                <div className="space-y-2">
                  <div className="flex items-center space-x-1">
                    {[...Array(5)].map((_, i) => (
                      <Star
                        key={i}
                        className={`w-4 h-4 ${
                          i < Math.floor(product.rating)
                            ? 'text-yellow-400 fill-current'
                            : 'text-gray-300'
                        }`}
                      />
                    ))}
                    <span className="text-sm text-gray-600 ml-2">({product.rating})</span>
                  </div>
                  <h4 className="font-bold text-gray-900">{product.name}</h4>
                  <p className="text-xl font-bold text-gray-900">${product.price}</p>
                </div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Motivational Section */}
      <section 
        className="relative py-32 bg-fixed bg-cover bg-center"
        style={{
          backgroundImage: 'url(https://images.unsplash.com/photo-1549060279-7e168fcee0c2?w=1920&h=800&fit=crop)'
        }}
      >
        <div className="absolute inset-0 bg-black opacity-60" />
        <div className="relative container mx-auto px-4 text-center text-white">
          <h3 className="text-5xl font-black mb-6">NO EXCUSES. JUST RESULTS.</h3>
          <p className="text-xl mb-8 max-w-2xl mx-auto">
            Join the SweatDrip community and transform your fitness journey with gear that performs as hard as you do.
          </p>
          <button className="bg-red-500 text-white px-8 py-4 font-bold hover:bg-red-600 transition-all transform hover:scale-105">
            START YOUR JOURNEY
          </button>
        </div>
      </section>

      {/* Brand Values */}
      <section className="py-20 bg-gray-900 text-white">
        <div className="container mx-auto px-4">
          <div className="text-center mb-16">
            <h3 className="text-4xl font-black mb-4">WHY CHOOSE SWEATDRIP</h3>
            <p className="text-gray-400 max-w-2xl mx-auto">
              We're more than just activewear. We're your partner in achieving greatness.
            </p>
          </div>
          
          <div className="grid md:grid-cols-3 gap-8">
            {[
              {
                title: 'PERFORMANCE DRIVEN',
                description: 'Advanced fabrics that wick moisture, stretch with you, and maintain shape through intense workouts.',
                image: 'https://images.unsplash.com/photo-1518310383802-640c2de311b2?w=600&h=400&fit=crop'
              },
              {
                title: 'SUSTAINABLE QUALITY',
                description: 'Eco-conscious materials and ethical manufacturing without compromising on durability or style.',
                image: 'https://images.unsplash.com/photo-1595909315417-2edd382a56dc?w=600&h=400&fit=crop'
              },
              {
                title: 'ATHLETE TESTED',
                description: 'Designed with input from professional athletes and tested in real training conditions.',
                image: 'https://images.unsplash.com/photo-1517963879433-6ad2b056d712?w=600&h=400&fit=crop'
              }
            ].map((value, index) => (
              <div key={index} className="group">
                <div className="relative h-48 mb-6 overflow-hidden rounded-lg">
                  <img 
                    src={value.image} 
                    alt={value.title}
                    className="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500"
                  />
                  <div className="absolute inset-0 bg-gradient-to-t from-black to-transparent opacity-40" />
                </div>
                <h4 className="text-xl font-bold mb-3">{value.title}</h4>
                <p className="text-gray-400">{value.description}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Testimonials */}
      <section className="py-20 bg-white">
        <div className="container mx-auto px-4">
          <div className="text-center mb-12">
            <h3 className="text-4xl font-black mb-4">COMMUNITY REVIEWS</h3>
            <p className="text-gray-600">Join thousands of athletes who trust SweatDrip</p>
          </div>
          
          <div className="grid md:grid-cols-3 gap-8">
            {[
              {
                name: 'Sarah M.',
                review: 'The quality is incredible! These leggings have become my go-to for every workout. They never lose shape.',
                rating: 5,
                avatar: 'https://images.unsplash.com/photo-1594381898411-846e7d193883?w=100&h=100&fit=crop'
              },
              {
                name: 'Mike T.',
                review: 'Finally found gym wear that looks as good as it performs. The fit is perfect and the material is top-notch.',
                rating: 5,
                avatar: 'https://images.unsplash.com/photo-1583468982228-19f19164aee2?w=100&h=100&fit=crop'
              },
              {
                name: 'Jessica L.',
                review: 'Love the attention to detail and the sustainable approach. Feels great to support a brand that cares.',
                rating: 5,
                avatar: 'https://images.unsplash.com/photo-1518310952931-b1de897abd40?w=100&h=100&fit=crop'
              }
            ].map((testimonial, index) => (
              <div key={index} className="bg-gray-50 p-6 rounded-lg">
                <div className="flex items-center mb-4">
                  <img 
                    src={testimonial.avatar} 
                    alt={testimonial.name}
                    className="w-12 h-12 rounded-full mr-4 object-cover"
                  />
                  <div className="flex">
                    {[...Array(testimonial.rating)].map((_, i) => (
                      <Star key={i} className="w-5 h-5 text-yellow-400 fill-current" />
                    ))}
                  </div>
                </div>
                <p className="text-gray-700 mb-4 italic">"{testimonial.review}"</p>
                <p className="font-bold text-gray-900">— {testimonial.name}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Instagram Feed */}
      <section className="py-20 bg-gray-100">
        <div className="container mx-auto px-4">
          <div className="text-center mb-12">
            <h3 className="text-4xl font-black mb-4">#SWEATDRIPFAM</h3>
            <p className="text-gray-600">Tag us @sweatdrip to be featured</p>
          </div>
          
          <div className="grid grid-cols-2 md:grid-cols-4 gap-4">
            {[
              'https://images.unsplash.com/photo-1541534741688-6078c6bfb5c5?w=400&h=400&fit=crop',
              'https://images.unsplash.com/photo-1550345332-09e3ac987658?w=400&h=400&fit=crop',
              'https://images.unsplash.com/photo-1518310916931-17d7d1e2c342?w=400&h=400&fit=crop',
              'https://images.unsplash.com/photo-1549476464-37392f717541?w=400&h=400&fit=crop',
              'https://images.unsplash.com/photo-1518611012118-696072aa579a?w=400&h=400&fit=crop',
              'https://images.unsplash.com/photo-1581009146145-b5ef050c2e1e?w=400&h=400&fit=crop',
              'https://images.unsplash.com/photo-1518310383802-640c2de311b2?w=400&h=400&fit=crop',
              'https://images.unsplash.com/photo-1517836357463-d25dfeac3438?w=400&h=400&fit=crop'
            ].map((image, index) => (
              <div key={index} className="relative group cursor-pointer overflow-hidden">
                <img 
                  src={image} 
                  alt={`Instagram ${index + 1}`}
                  className="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500"
                />
                <div className="absolute inset-0 bg-black opacity-0 group-hover:opacity-40 transition-opacity flex items-center justify-center">
                  <Heart className="w-8 h-8 text-white opacity-0 group-hover:opacity-100 transition-opacity" />
                </div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Newsletter */}
      <section className="py-20 bg-red-500">
        <div className="container mx-auto px-4 text-center">
          <h3 className="text-4xl font-black text-white mb-4">JOIN THE MOVEMENT</h3>
          <p className="text-white text-xl mb-8 opacity-90">
            Get exclusive access to new drops, training tips, and member-only discounts
          </p>
          <form className="max-w-md mx-auto flex gap-4" onSubmit={(e) => e.preventDefault()}>
            <input
              type="email"
              value={email}
              onChange={(e) => setEmail(e.target.value)}
              placeholder="Enter your email"
              className="flex-1 px-6 py-3 rounded-full text-gray-900 font-medium focus:outline-none focus:ring-4 focus:ring-white focus:ring-opacity-50"
            />
            <button className="bg-gray-900 text-white px-8 py-3 rounded-full font-bold hover:bg-gray-800 transition-colors">
              SUBSCRIBE
            </button>
          </form>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-gray-900 text-white py-16">
        <div className="container mx-auto px-4">
          <div className="grid md:grid-cols-4 gap-8 mb-8">
            <div>
              <h4 className="font-bold text-xl mb-4">Sweat<span className="text-red-500">Drip</span></h4>
              <p className="text-gray-400">Elevate your performance with premium activewear designed for champions.</p>
            </div>
            <div>
              <h5 className="font-bold mb-4">SHOP</h5>
              <ul className="space-y-2 text-gray-400">
                <li><button className="hover:text-white transition-colors">Women</button></li>
                <li><button className="hover:text-white transition-colors">Men</button></li>
                <li><button className="hover:text-white transition-colors">New Arrivals</button></li>
                <li><button className="hover:text-white transition-colors">Sale</button></li>
              </ul>
            </div>
            <div>
              <h5 className="font-bold mb-4">HELP</h5>
              <ul className="space-y-2 text-gray-400">
                <li><button className="hover:text-white transition-colors">Size Guide</button></li>
                <li><button className="hover:text-white transition-colors">Shipping</button></li>
                <li><button className="hover:text-white transition-colors">Returns</button></li>
                <li><button className="hover:text-white transition-colors">Contact Us</button></li>
              </ul>
            </div>
            <div>
              <h5 className="font-bold mb-4">CONNECT</h5>
              <ul className="space-y-2 text-gray-400">
                <li><button className="hover:text-white transition-colors">Instagram</button></li>
                <li><button className="hover:text-white transition-colors">Facebook</button></li>
                <li><button className="hover:text-white transition-colors">Twitter</button></li>
                <li><button className="hover-white transition-colors">YouTube</button></li>
              </ul>
            </div>
          </div>
          <div className="border-t border-gray-800 pt-8 text-center text-gray-400">
            <p>&copy; 2024 SweatDrip. All rights reserved.</p>
          </div>
        </div>
      </footer>

      {/* Product Modal */}
      {selectedProduct && (
        <div className="fixed inset-0 bg-black bg-opacity-50 z-50 flex items-center justify-center p-4" onClick={() => setSelectedProduct(null)}>
          <div className="bg-white rounded-lg max-w-2xl w-full max-h-screen overflow-y-auto" onClick={(e) => e.stopPropagation()}>
            <div className="p-6">
              <div className="flex justify-between items-start mb-4">
                <h3 className="text-2xl font-bold">{selectedProduct.name}</h3>
                <button onClick={() => setSelectedProduct(null)} className="p-2 hover:bg-gray-100 rounded-full">
                  <X className="w-5 h-5" />
                </button>
              </div>
              
              <div className="grid md:grid-cols-2 gap-6">
                <div className="aspect-square rounded-lg overflow-hidden">
                  <img 
                    src={selectedProduct.image} 
                    alt={selectedProduct.name}
                    className="w-full h-full object-cover"
                  />
                </div>
                
                <div className="space-y-4">
                  <div className="flex items-center space-x-2">
                    {[...Array(5)].map((_, i) => (
                      <Star
                        key={i}
                        className={`w-5 h-5 ${
                          i < Math.floor(selectedProduct.rating)
                            ? 'text-yellow-400 fill-current'
                            : 'text-gray-300'
                        }`}
                      />
                    ))}
                    <span className="text-gray-600">({selectedProduct.rating})</span>
                  </div>
                  
                  <p className="text-3xl font-bold">${selectedProduct.price}</p>
                  
                  <div>
                    <p className="font-medium mb-2">Select Size:</p>
                    <div className="flex gap-2">
                      {['XS', 'S', 'M', 'L', 'XL'].map((size) => (
                        <button
                          key={size}
                          onClick={() => setSelectedSize(size)}
                          className={`w-12 h-12 border-2 font-medium transition-all ${
                            selectedSize === size
                              ? 'border-gray-900 bg-gray-900 text-white'
                              : 'border-gray-300 hover:border-gray-400'
                          }`}
                        >
                          {size}
                        </button>
                      ))}
                    </div>
                  </div>
                  
                  <button
                    onClick={() => addToCart(selectedProduct)}
                    disabled={!selectedSize}
                    className={`w-full py-3 font-bold transition-all ${
                      selectedSize
                        ? 'bg-gray-900 text-white hover:bg-gray-800'
                        : 'bg-gray-200 text-gray-400 cursor-not-allowed'
                    }`}
                  >
                    {selectedSize ? 'ADD TO CART' : 'SELECT SIZE'}
                  </button>
                  
                  <div className="space-y-2 pt-4 border-t">
                    <div className="flex items-center gap-2">
                      <Check className="w-5 h-5 text-green-500" />
                      <span className="text-sm">Free shipping on orders over $100</span>
                    </div>
                    <div className="flex items-center gap-2">
                      <Check className="w-5 h-5 text-green-500" />
                      <span className="text-sm">30-day return policy</span>
                    </div>
                    <div className="flex items-center gap-2">
                      <Check className="w-5 h-5 text-green-500" />
                      <span className="text-sm">Lifetime warranty</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      )}

      {/* Cart Sidebar */}
      <div className={`fixed right-0 top-0 h-full w-96 bg-white shadow-2xl z-50 transform transition-transform ${
        cartOpen ? 'translate-x-0' : 'translate-x-full'
      }`}>
        <div className="flex flex-col h-full">
          <div className="flex items-center justify-between p-6 border-b">
            <h3 className="text-xl font-bold">Shopping Cart ({cartCount})</h3>
            <button onClick={() => setCartOpen(false)} className="p-2 hover:bg-gray-100 rounded-full">
              <X className="w-5 h-5" />
            </button>
          </div>
          
          <div className="flex-1 overflow-y-auto p-6">
            {cart.length === 0 ? (
              <p className="text-gray-500 text-center py-8">Your cart is empty</p>
            ) : (
              <div className="space-y-4">
                {cart.map((item) => (
                  <div key={`${item.id}-${item.size}`} className="flex gap-4 pb-4 border-b">
                    <img 
                      src={item.image} 
                      alt={item.name}
                      className="w-20 h-20 object-cover rounded"
                    />
                    <div className="flex-1">
                      <h4 className="font-medium">{item.name}</h4>
                      <p className="text-sm text-gray-600">Size: {item.size}</p>
                      <p className="font-bold">${item.price}</p>
                    </div>
                    <div className="flex items-center gap-2">
                      <button
                        onClick={() => updateQuantity(item.id, item.size, -1)}
                        className="w-8 h-8 border rounded hover:bg-gray-100"
                      >
                        <Minus className="w-4 h-4 mx-auto" />
                      </button>
                      <span className="w-8 text-center">{item.quantity}</span>
                      <button
                        onClick={() => updateQuantity(item.id, item.size, 1)}
                        className="w-8 h-8 border rounded hover:bg-gray-100"
                      >
                        <Plus className="w-4 h-4 mx-auto" />
                      </button>
                    </div>
                  </div>
                ))}
              </div>
            )}
          </div>
          
          {cart.length > 0 && (
            <div className="border-t p-6 space-y-4">
              <div className="flex justify-between text-xl font-bold">
                <span>Total</span>
                <span>${cartTotal}</span>
              </div>
              <button className="w-full bg-gray-900 text-white py-3 font-bold hover:bg-gray-800 transition-colors">
                CHECKOUT
              </button>
            </div>
          )}
        </div>
      </div>

      {/* Mobile Menu */}
      {mobileMenuOpen && (
        <div className="fixed inset-0 bg-white z-40 md:hidden">
          <div className="p-6">
            <div className="flex justify-between items-center mb-8">
              <h2 className="text-2xl font-black">Sweat<span className="text-red-500">Drip</span></h2>
              <button onClick={() => setMobileMenuOpen(false)}>
                <X className="w-6 h-6" />
              </button>
            </div>
            <nav className="space-y-4">
              {['New Arrivals', 'Women', 'Men', 'Collections', 'Sale'].map((item) => (
                <button
                  key={item}
                  className="block w-full text-left text-xl font-medium py-2 hover:text-red-500 transition-colors"
                  onClick={() => setMobileMenuOpen(false)}
                >
                  {item}
                </button>
              ))}
            </nav>
          </div>
        </div>
      )}
    </div>
  );
}
