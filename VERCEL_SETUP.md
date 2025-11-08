# Vercel Deployment Kurulumu

## Private Repository için Vercel Kurulumu

### Adım 1: Vercel'e GitHub Erişim İzni Verin

1. Vercel dashboard'a gidin: https://vercel.com/dashboard
2. Sağ üstteki profil ikonuna tıklayın
3. "Settings" (Ayarlar) seçeneğine gidin
4. Sol menüden "Git" sekmesine tıklayın
5. "GitHub" bölümünde "Configure" veya "Connect" butonuna tıklayın
6. GitHub'da açılan pencerede:
   - "Authorize Vercel" butonuna tıklayın
   - **ÖNEMLİ**: "Private repositories" seçeneğini işaretleyin
   - İzinleri onaylayın

### Adım 2: Repository'yi Import Edin

1. Vercel dashboard'da "Add New..." > "Project" butonuna tıklayın
2. "Import Git Repository" bölümünde:
   - "Select a Git Namespace" dropdown'ından GitHub hesabınızı seçin
   - "Search..." kutusuna `Alican_LawyerBlog` yazın
   - Repository'nizi bulun ve seçin
3. "Import" butonuna tıklayın

### Adım 3: Build Ayarları

Vercel otomatik olarak Next.js projesini algılayacak:
- Framework Preset: Next.js
- Build Command: `npm run build` (otomatik)
- Output Directory: `.next` (otomatik)
- Install Command: `npm install` (otomatik)

### Adım 4: Deploy

1. "Deploy" butonuna tıklayın
2. 1-2 dakika içinde projeniz canlıda olacak!

## Alternatif: Repository'yi Public Yapmak

Eğer repository'yi public yapmak isterseniz:

1. GitHub repository sayfasına gidin
2. "Settings" sekmesine tıklayın
3. En alta inin ve "Danger Zone" bölümünü bulun
4. "Change visibility" > "Make public" seçeneğini seçin
5. Repository adını yazarak onaylayın

**Not**: Public yapmak istemiyorsanız, yukarıdaki GitHub erişim izni yöntemini kullanın.

