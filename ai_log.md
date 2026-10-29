bu dosyaya web projesi dersi boyunca hafta hafta yapayzekaya yazdığımız promptları ve bize verdiği cevapları ve bu cevaplardan 
nasıl faydalandığımız not etcez
16 ekim görevi
ai a sorduğum soru
verdiği cevap
ve bu cevabı nasıl kullandığımız
14.10.26 Çarşamba
soru: Web proje dersi için proje yapmam gerekiyor ne yapabilirim örneklendirme ver
cevap: Nerede Ne Yenir Mekan ve Lezzet Rehberi 
Konu: Kullanıcıların şehir bazlı veya yemek türüne göre mekan sorguladığı bi platform
Özellikler: Mekan filtreleme (katagori,fiyat,puan)
            Kullanıcı yorumu 
            Harita üzerinde mekanları gösterme
            29.10.26 Perşembe
            soru:NERDE NE YENİR WEB SİTESİ TASARLAMAM LAZIM
            cevap:"Nerde Ne Yenir" sitesini tasarlıyorum — önce ödevin tam isteklerini netleştirip ona uygun kuruyorum.

NerdeNeYenir sitesini tasarlandı
"Nerde Ne Yenir" sitesi tam olarak nasıl olsun?
Restoran keşif sitesi
Site örnek verilerle mi çalışsın, kullanıcılar da katkı verebilsin mi?
Kullanıcı katılımı olsun
Az önce yaptığımız QR menü ne olsun?
Onu tamamen değiştir
Giriş yapan kullanıcıların isim/avatar gibi profil bilgisi olsun mu?
Profil olsun
Hangi özellikler olsun? (birden fazla seçebilirsin)
Şehir & kategori filtresi, Yorumlar, Puanlama, Favoriler
soru:BANA ŞUAN BU SİTENİN SADECE SİTENİN ÖN YÜZÜ LAZIM
cevap:Anlıyorum — şimdi tamamen ön yüze odaklanıyorum: ana sayfa, filtreler, mekan kartları ve detay sayfası. Örnek mekanlar hazır veritabanından geldiği için arayüz anında dolu görünecek.
kod: import { Search } from "lucide-react";
import type { CategoryItem } from "@/restaurants.functions";

type Filters = { city?: string; category?: string; q?: string };
type Filters = { sehir?: string; kategori?: string; q?: string };

export function FilterBar({
  categories,
  />
        </form>
        <select
          value={filters.city ?? ""}
          onChange={(e) => apply({ city: e.target.value || undefined })}
          value={filters.sehir ?? ""}
          onChange={(e) => apply({ sehir: e.target.value || undefined })}
          className="h-11 rounded-full border border-input bg-card px-4 text-sm text-foreground outline-none focus:border-ring focus:ring-2 focus:ring-ring/30"
        >
          <option value="">Tüm şehirler</option>
          <div className="no-scrollbar flex gap-2 overflow-x-auto pb-1">
        <button
          onClick={() => apply({ category: undefined })}
          onClick={() => apply({ kategori: undefined })}
          className={`shrink-0 rounded-full border px-4 py-1.5 text-xs font-semibold transition-colors ${
            !filters.category
            !filters.kategori
              ? "border-primary bg-primary text-primary-foreground"
              : "border-border bg-card text-muted-foreground hover:border-primary hover:text-primary"
          }`}
          <button
            key={c.slug}
            onClick={() =>
              apply({ category: filters.category === c.slug ? undefined : c.slug })
              apply({ kategori: filters.kategori === c.slug ? undefined : c.slug })
            }
            className={`shrink-0 rounded-full border px-4 py-1.5 text-xs font-semibold transition-colors ${
              filters.category === c.slug
              filters.kategori === c.slug
                ? "border-primary bg-primary text-primary-foreground"
                : "border-border bg-card text-muted-foreground hover:border-primary hover:text-primary"
            }`}
          
  


