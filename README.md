# PetLove - Evcil Hayvan Sahiplendirme Uygulaması

Modern ve şık bir React Native uygulaması. TypeScript ile geliştirilmiş, evcil hayvan sahiplendirme için özelleştirilmiş filtreleme seçenekleri ile yeni dostunuz ile tanışın.

## ✨ Özellikler

- **Evcil Hayvanları Keşfet**: Sahiplenmeye uygun evcil hayvanların özenle seçilmiş koleksiyonuna göz atın
- **Gelişmiş Filtreleme**: Hayvan türü, yaş ve konuma göre filtreleme yapın
- **Favoriler Sistemi**: İlginizi çeken hayvanları kolay erişim için kaydedin
- **Detaylı Profiller**: Hayvanların hikayeleri, özellikleri ve barınak bilgileri dahil kapsamlı bilgiler
- **Başvuru Sistemi**: Uygulama üzerinden barınaklarla doğrudan iletişime geçin
- **Bakım Kaynakları**: Evcil hayvan bakımı için eğitim içerikleri ve ipuçları
- **Kullanıcı Profilleri**: Sahiplenme sürecinizi ve kaydedilen hayvanları takip edin

## 🛠 Kullanılan Teknolojiler

- **React** (hooks ile birlikte)
- **React Router DOM** – istemci tarafı yönlendirme
- **Firebase** – kimlik doğrulama ve gerçek zamanlı veritabanı
- **React Hook Form + Yup** – formlar ve doğrulama
- **React Modal** – deneme dersi için modal pencere
- **React Hot Toast** – bildirimler
- **Axios** – veri çekme işlemleri
- **CSS Modules** – bileşenlere özel stillendirme

## 📁 Project Structure

```
PetLove/
├── app/                    # Expo Router app directory
│   ├── _layout.tsx        # Root layout with font loading
│   ├── (tabs)/            # Tab navigation
│   │   ├── _layout.tsx    # Tab layout configuration
│   │   ├── index.tsx      # Discover screen
│   │   ├── favorites.tsx  # Favorites screen
│   │   ├── care.tsx       # Care resources screen
│   │   └── profile.tsx    # User profile screen
│   ├── pet/               # Pet detail routes
│   │   └── [id].tsx      # Dynamic pet detail screen
│   └── +not-found.tsx    # 404 error page
├── components/            # Reusable UI components
│   ├── PetCard.tsx       # Pet listing card component
│   ├── FilterModal.tsx   # Filter modal component
│   └── InquiryModal.tsx  # Contact form modal
├── data/                 # Mock data and types
│   └── mockPets.ts      # Sample pet data
├── hooks/               # Custom React hooks
│   └── useFrameworkReady.ts
├── utils/               # Utility functions
│   └── favorites.ts     # Favorites management
├── assets/              # Static assets
│   └── images/         # App icons and images
└── docs/               # Documentation
    ├── ARCHITECTURE.md  # Architecture documentation
    ├── API.md          # API documentation
    └── DEPLOYMENT.md   # Deployment guide
```

### 1. Repoyu klonlayın:

```bash
git https://github.com/ferhatipek/petlove.git
cd petlove-app-main
npm install
npm