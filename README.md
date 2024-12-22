# Classification of Animals

Bu proje, hayvanları sınıflandırmak için çeşitli teknikleri gösteren bir Jupyter Notebook'tur.

### Bölüm 1

#   * * V e r i   S e t i   H a z ı r l a m a   S ü r e c i * * 
 B u   b e t i k ,   v e r i   s e t i n i   e ğ i t i m   i ç i n   h a z ı r l a m a k   a m a c ı y l a   a ş a ğ ı d a k i   a d ı m l a r ı   g e r ç e k l e ş t i r i r : 
 
 1 .   * * V e r i   S e t i   D i z i n i   v e   S ı n ı f   S e ç i m i * * 
 *   V e r i   S e t i   D i z i n l e r i : 
 G i r d i ,   ç ı k t ı   v e   i ş l e n m i ş   v e r i   d i z i n l e r i n i   t a n ı m l a r . 
 *   S ı n ı f   S e ç i m i : 
 P r o j e d e   k u l l a n ı l a c a k   h a y v a n   s ı n ı f l a r ı n ı   b e l i r l e r . 
 
 2 .   * * G ö r ü n t ü   S ı n ı r l a r ı   v e   Ö n   İ ş l e m e   A y a r l a r ı * * 
 *   S ı n ı f   B a ş ı n a   G ö r ü n t ü   S ı n ı r ı : 
 H e r   s ı n ı f   i ç i n   m a k s i m u m   6 5 0   g ö r ü n t ü   i l e   s ı n ı r l a n d ı r ı r . 
 *   G ö r ü n t ü   B o y u t l a n d ı r m a : 
 G ö r ü n t ü l e r i   y e n i d e n   b o y u t l a n d ı r m a k   i ç i n   h e d e f   b o y u t u   ( ö r n e ğ i n ,   1 2 8 x 1 2 8   p i k s e l )   a y a r l a r . 
 
 3 .   * * Ç ı k t ı   D i z i n l e r i n i n   K u r u l u m u * * 
 *   M e v c u t   D i z i n l e r i n   T e m i z l e n m e s i : 
 Ç ı k t ı   v e   i ş l e n m i ş   v e r i   d i z i n l e r i n i   t e m i z l e y e r e k   i ş l e m   ö n c e s i   t e m i z   b i r   b a ş l a n g ı ç   s a ğ l a r . 
 *   Y e n i   D i z i n l e r i n   O l u ş t u r u l m a s ı : 
 İ ş l e n m i ş   g ö r ü n t ü l e r i n   k a y d e d i l m e s i   i ç i n   g e r e k l i   o l a n   d i z i n l e r i   y e n i d e n   o l u ş t u r u r . 
 
 4 .   * * G ö r ü n t ü   K o p y a l a m a   v e   İ ş l e m e * * 
 *   S ı n ı f l a r   A r a s ı n d a   Y i n e l e m e : 
 B e l i r t i l e n   h a y v a n   s ı n ı f l a r ı   a r a s ı n d a   d ö n g ü   y a p a r . 
 *   G ö r ü n t ü l e r i n   Ç ı k t ı   D i z i n i n e   K o p y a l a n m a s ı : 
 H e r   s ı n ı f   i ç i n   b e l i r t i l e n   s ı n ı r a   k a d a r   o l a n   g ö r ü n t ü l e r i   ç ı k t ı   d i z i n i n e   k o p y a l a r . 
 *   G ö r ü n t ü l e r i n   İ ş l e n m e s i : 
 G ö r ü n t ü l e r i   y e n i d e n   b o y u t l a n d ı r ı r   v e   n o r m a l l e ş t i r e r e k   i ş l e n m i ş   d i z i n e   k a y d e d e r .
### Bölüm 2

#   * * E ğ i t i m   v e   T e s t   V e r i l e r i n i n   H a z ı r l a n m a s ı * * 
 B u   b e t i k ,   v e r i   s e t i n i   e ğ i t i m   v e   t e s t   i ç i n   h a z ı r l a m a k   a m a c ı y l a   a ş a ğ ı d a k i   i ş l e m l e r i   g e r ç e k l e ş t i r i r : 
 
 1 .   * * V e r i   S e t i   v e   E t i k e t l e r i n   T a n ı m l a n m a s ı * * 
 *   İ ş l e n m i ş   V e r i   S e t i   D i z i n i : 
 İ ş l e n m i ş   v e r i   s e t i   d i z i n i n i   t a n ı m l a r . 
 *   H a y v a n   S ı n ı f l a r ı   v e   E t i k e t l e r : 
 S e ç i l e n   h a y v a n   s ı n ı f l a r ı n ı   l i s t e l e r   v e   b u   s ı n ı f l a r ı   s a y ı s a l   e t i k e t l e r e   d ö n ü ş t ü r ü r . 
 
 2 .   * * V e r i   Y ü k l e m e   v e   N o r m a l i z a s y o n * * 
 *   G ö r ü n t ü l e r i n   İ ş l e n m e s i : 
 H e r   s e ç i l e n   s ı n ı f   i ç i n   i ş l e n m i ş   g ö r ü n t ü l e r   ü z e r i n d e   i t e r a s y o n   y a p a r . 
 *   P i k s e l   D e ğ e r l e r i n i n   N o r m a l i z a s y o n u : 
 G ö r ü n t ü l e r i n   p i k s e l   d e ğ e r l e r i n i   [ 0 ,   1 ]   a r a l ı ğ ı n a   d ö n ü ş t ü r ü r . 
 
 3 .   * * V e r i l e r i n   D ö n ü ş t ü r ü l m e s i * * 
 *   N u m P y   D ö n ü ş ü m ü : 
 G ö r ü n t ü   v e   e t i k e t   l i s t e l e r i n i   m o d e l l e   u y u m l u   h a l e   g e t i r m e k   i ç i n   N u m P y   d i z i l e r i n e   d ö n ü ş t ü r ü r . 
 
 4 .   * * V e r i   S e t i n i n   B ö l ü n m e s i * * 
 *   E ğ i t i m   v e   T e s t   A y r ı m ı : 
 V e r i   s e t i n i   % 7 0   e ğ i t i m   v e   % 3 0   t e s t   o l a c a k   ş e k i l d e   b ö l e r . 
 *   R a s t g e l e l i k   K o n t r o l ü : 
 S a b i t   b i r   r a s t g e l e l i k   t o h u m u   k u l l a n a r a k   b ö l ü n m e n i n   r e p r o d u c i b l e   ( t e k r a r l a n a b i l i r )   o l m a s ı n ı   s a ğ l a r . 

### Bölüm 3

#   * * E ğ i t i m   V e r i l e r i   İ ç i n   V e r i   A r t ı r ı m ı   ( D a t a   A u g m e n t a t i o n ) * * 
 1 .   * * V e r i   A r t ı r ı m ı   B a ş l a t ı l m a s ı * * 
 *   I m a g e D a t a G e n e r a t o r   s ı n ı f ı n ı n   b i r   ö r n e ğ i ,   a ş a ğ ı d a k i   v e r i   a r t ı r ı m ı   s e ç e n e k l e r i y l e   o l u ş t u r u l u r : 
 *   * * D ö n d ü r m e   ( R o t a t i o n ) : * *   ± 2 0   d e r e c e   a r a s ı n d a   r a s t g e l e   d ö n d ü r m e . 
 *   * * Y a t a y   v e   D i k e y   K a y d ı r m a : * *   G ö r ü n t ü l e r i   t o p l a m   g e n i ş l i ğ i n   v e y a   y ü k s e k l i ğ i n   % 2 0 ' s i   k a d a r   r a s t g e l e   k a y d ı r m a . 
 *   * * K e s m e   D ö n ü ş ü m l e r i   ( S h e a r   T r a n s f o r m a t i o n s ) : * *   R a s t g e l e   k e s m e   d ö n ü ş ü m l e r i   u y g u l a n m a s ı . 
 *   * * Y a k ı n l a ş t ı r m a   ( Z o o m ) : * *   G ö r ü n t ü l e r e   % 2 0   o r a n ı n d a   r a s t g e l e   y a k ı n l a ş t ı r m a . 
 *   * * Y a t a y   Ç e v i r m e   ( H o r i z o n t a l   F l i p ) : * *   G ö r ü n t ü l e r i   y a t a y   e k s e n d e   r a s t g e l e   ç e v i r m e . 
 *   * * D o l d u r m a   M o d u   ( F i l l   M o d e ) : * *   D ö n ü ş ü m l e r   s o n r a s ı   o l u ş a n   b o ş   p i k s e l l e r i n   n a s ı l   d o l d u r u l a c a ğ ı n ı   b e l i r t i r . 
 
 2 .   * * V e r i   A r t ı r ı m ı   U y g u l a n m a s ı * * 
 *   E ğ i t i m   g ö r ü n t ü l e r i   ( X _ t r a i n )   v e   b u n l a r a   k a r ş ı l ı k   g e l e n   e t i k e t l e r   ( y _ t r a i n ) ,   3 2   g ö r ü n t ü l ü k   p a r t i l e r   h a l i n d e   a r t ı r ı l ı r . 
 
 3 .   * * Ç ı k t ı * * 
 *   E ğ i t i m   v e r i l e r i n e   v e r i   a r t ı r ı m ı   i ş l e m i n i n   b a ş a r ı y l a   u y g u l a n d ı ğ ı   d o ğ r u l a n ı r .
### Bölüm 4

#   * * G ö r ü n t ü   M a n i p ü l a s y o n u   v e   B e y a z   D e n g e s i   D ü z e l t m e * * 
 
 B u   b e t i k ,   g ö r ü n t ü   v e r i   s e t l e r i   ü z e r i n d e   i k i   t e m e l   i ş l e m i   g e r ç e k l e ş t i r i r : 
 
 1 .   * * G ö r ü n t ü   M a n i p ü l a s y o n u * *   
       -   P a r l a k l ı k   v e   k o n t r a s t   a y a r l a r ı n ı   d e ğ i ş t i r e r e k   ç e ş i t l i   ı ş ı k l a n d ı r m a   k o ş u l l a r ı n ı   s i m ü l e   e d e r . 
       -   M a n i p ü l e   e d i l m i ş   g ö r ü n t ü l e r i   b e l i r t i l e n   ç ı k t ı   d i z i n i n e   k a y d e d e r . 
 
 2 .   * * B e y a z   D e n g e s i   D ü z e l t m e s i   U y g u l a m a * * 
       -   G r a y   W o r l d   ( G r i   D ü n y a )   v a r s a y ı m ı n ı   k u l l a n a r a k   g ö r ü n t ü l e r d e k i   r e n k l e r i   n o r m a l i z e   e d e r . 
       -   R G B   k a n a l l a r ı n ı n   o r t a l a m a   y o ğ u n l u k l a r ı n a   g ö r e   p i k s e l   d e ğ e r l e r i n i   a y a r l a r . 
 
 # #   * * G ö r ü n t ü   M a n i p ü l a s y o n u * * 
 
 # # #   * * G e n e l   B a k ı ş * * 
 ` g e t _ m a n i p u l a t e d _ i m a g e s `   f o n k s i y o n u : 
 -   B e l i r t i l e n   g i r i ş   d i z i n i n d e k i   t ü m   g ö r ü n t ü l e r   i ç i n   p a r l a k l ı k   v e   k o n t r a s t   a y a r l a r ı n ı   d ü z e n l e r . 
 -   M a n i p ü l e   e d i l m i ş   g ö r ü n t ü l e r i   b e l i r t i l e n   ç ı k t ı   d i z i n i n e   k a y d e d e r . 
 
 
 # # #   * * A n a h t a r   P a r a m e t r e l e r * * 
 -   * * P a r l a k l ı k   F a k t ö r ü   ( B r i g h t n e s s   F a c t o r ) * * :   G ö r ü n t ü l e r i n   g e n e l   p a r l a k l ı k   s e v i y e s i n i   k o n t r o l   e d e r . 
 -   * * K o n t r a s t   F a k t ö r ü   ( C o n t r a s t   F a c t o r ) * * :   G ö r ü n t ü l e r d e k i   k o y u   v e   a ç ı k   a l a n l a r   a r a s ı n d a k i   f a r k ı   a y a r l a r . 

### Bölüm 5

#   * * İ ş l e n m i ş   v e   B e y a z   D e n g e l i   V e r i   K ü m e l e r i n i n   Y ü k l e n m e s i * * 
 
 B u   b ö l ü m ,   i ş l e n m i ş   v e   b e y a z   d e n g e l i   v e r i   k ü m e l e r i n i n   e ğ i t i m   v e y a   d e ğ e r l e n d i r m e d e   d a h a   f a z l a   k u l l a n ı m   i ç i n   n a s ı l   y ü k l e n e c e ğ i n i   g ö s t e r i r .
### Bölüm 6

#   * * V e r i   K ü m e l e r i n i   B i r l e ş t i r m e   v e   M o d e l i   E ğ i t m e * * 
 
 B u   b ö l ü m ,   v e r i   k ü m e l e r i n i   ( o r i j i n a l ,   i ş l e n m i ş   v e   b e y a z   d e n g e l i )   b i r l e ş t i r m e   v e   b i r l e ş t i r i l m i ş   v e r i l e r   ü z e r i n d e   b i r   C N N   m o d e l i   e ğ i t m e   s ü r e c i n i   g ö s t e r i r . 
 
 - - - 
 
 # #   * * V e r i   K ü m e l e r i n i   B i r l e ş t i r m e * * 
 
 # # #   * * G e n e l   B a k ı ş * * 
 -   O r i j i n a l ,   i ş l e n m i ş   v e   b e y a z   d e n g e l i   v e r i   k ü m e l e r i   t e k   b i r   v e r i   k ü m e s i n d e   b i r l e ş t i r i l i r . 
 -   M o d e l i n   ç e ş i t l i   v e r i   d a ğ ı t ı m l a r ı n d a n   ö ğ r e n m e s i n i   s a ğ l a r . 
 
 # # #   * * K o d * * 
 ` ` ` p y t h o n 
 #   O r i j i n a l ,   İ ş l e n m i ş   v e   B e y a z   D e n g e l i   V e r i   K ü m e l e r i n i   B i r l e ş t i r m e 
 X _ c o m b i n e d _ t r a i n   =   n p . c o n c a t e n a t e ( [ X _ t r a i n ,   X _ m a n i p u l a t e d _ t r a i n ,   X _ w b _ t r a i n ] ,   a x i s = 0 ) 
 y _ c o m b i n e d _ t r a i n   =   n p . c o n c a t e n a t e ( [ y _ t r a i n ,   y _ m a n i p u l a t e d _ t r a i n ,   y _ w b _ t r a i n ] ,   a x i s = 0 ) 

### Bölüm 7

#   * * M o d e l i n   İ ş l e n m i ş   T e s t   S e t i n d e   D e ğ e r l e n d i r i l m e s i * * 
 
 # #   * * G e n e l   B a k ı ş * * 
 B u   b ö l ü m ,   p a r l a k l ı k   v e   k o n t r a s t   a y a r l a m a l a r ı   i ç e r e n   g ö r ü n t ü l e r   i ç e r e n   i ş l e n m i ş   t e s t   s e t i n d e k i   m o d e l i n   p e r f o r m a n s ı n ı   d e ğ e r l e n d i r i r .   A m a ç ,   m o d e l i n   d e ğ i ş t i r i l m i ş   ı ş ı k   k o ş u l l a r ı n a   n e   k a d a r   i y i   g e n e l l e ş t i r i l d i ğ i n i   d e ğ e r l e n d i r m e k t i r . 
 
 # #   * * A d ı m l a r * * 
 
 # # #   * * 1 .   İ ş l e n m i ş   T e s t   S e t i n i   Y ü k l e * * 
 -   İ ş l e n m i ş   v e r i   s e t i   b e l i r t i l e n   d i z i n d e n   y ü k l e n i r . 
 -   G ö r ü n t ü l e r   v e   e t i k e t l e r   ç ı k a r ı l ı r . 
 
 # # # #   * * K o d * * 
 ` ` ` p y t h o n 
 m a n i p u l a t e d _ d i r   =   " / k a g g l e / w o r k i n g / m a n i p u l a t e d _ i m a g e s "   #   G e r e k t i ğ i   g i b i   y o l u   a y a r l a y ı n 
 
 #   İ ş l e n m i ş   t e s t   g ö r ü n t ü l e r i n i   v e   e t i k e t l e r i n i   y ü k l e y i n 
 X _ m a n i p u l a t e d _ t e s t ,   y _ m a n i p u l a t e d _ t e s t   =   l o a d _ i m a g e s _ f r o m _ d i r e c t o r y ( m a n i p u l a t e d _ d i r ,   s e l e c t e d _ c l a s s e s ) 
 p r i n t ( f " M a n i p u l a t e d   T e s t   S e t   L o a d e d :   { X _ m a n i p u l a t e d _ t e s t . s h a p e } ,   { y _ m a n i p u l a t e d _ t e s t . s h a p e } " )
### Bölüm 8

#   * * B e y a z   D e n g e l i   T e s t   S e t i n d e   M o d e l i n   D e ğ e r l e n d i r i l m e s i * * 
 
 # #   * * G e n e l   B a k ı ş * * 
 B u   b ö l ü m ,   r e n k   n o r m a l i z a s y o n u   i ç i n   G r i   D ü n y a   v a r s a y ı m ı   k u l l a n ı l a r a k   i ş l e n e n   b e y a z   d e n g e l i   t e s t   s e t i n d e k i   m o d e l i n   p e r f o r m a n s ı n ı   d e ğ e r l e n d i r i r   M o d e l i n   a m a c ı   b e y a z   d e n g e s i   d ü z e l t m e s i n i n   s ı n ı f l a n d ı r m a   d o ğ r u l u ğ u n u   i y i l e ş t i r i p   i y i l e ş t i r m e d i ğ i n i   b e l i r l e m e k t i r . 
 
 # #   * * A d ı m l a r * * 
 
 # # #   * * 1 .   B e y a z   D e n g e l i   T e s t   S e t i n i   Y ü k l e * * 
 -   B e y a z   d e n g e l i   v e r i   s e t i   b e l i r t i l e n   d i z i n d e n   y ü k l e n i r . 
 -   G ö r ü n t ü l e r   v e   e t i k e t l e r   ç ı k a r ı l ı r . 
 
 # # # #   * * K o d * * 
 ` ` ` p y t h o n 
 w b _ o u t p u t _ d i r   =   " / k a g g l e / w o r k i n g / w b _ c o r r e c t e d _ i m a g e s "   #   Y o l u   g e r e k t i ğ i   g i b i   a y a r l a y ı n 
 
 #   B e y a z   d e n g e l i   t e s t   g ö r ü n t ü l e r i   v e   e t i k e t l e r i   y ü k l e y i n 
 X _ w b _ t e s t ,   y _ w b _ t e s t   =   l o a d _ i m a g e s _ f r o m _ d i r e c t o r y ( w b _ o u t p u t _ d i r ,   s e l e c t e d _ c l a s s e s ) 
 p r i n t ( f " W h i t e - B a l a n c e d   T e s t   S e t   L o a d e d :   { X _ w b _ t e s t . s h a p e } ,   { y _ w b _ t e s t . s h a p e } " ) 

### Bölüm 9

#   * * M o d e l i n   O r i j i n a l   T e s t   S e t i n d e   D e ğ e r l e n d i r i l m e s i * * 
 
 # #   * * G e n e l   B a k ı ş * * 
 B u   a d ı m d a ,   b i r   t e m e l   p e r f o r m a n s   b e l i r l e m e k   i ç i n   m o d e l i n   o r i j i n a l   ( d e ğ i ş t i r i l m e m i ş )   t e s t   v e r i   s e t i n d e k i   p e r f o r m a n s ı n ı   d e ğ e r l e n d i r i y o r u z . 
 
 # #   * * A d ı m l a r * * 
 
 # # #   * * 1 .   E t i k e t l e r i   T e k   S ı c a k   K o d l a m a y a   D ö n ü ş t ü r * * 
 -   E t i k e t l e r ,   k a t e g o r i k   s ı n ı f l a n d ı r m a   m o d e l i y l e   u y u m l u l u k   i ç i n   t e k   s ı c a k   k o d l a n m ı ş   b i r   b i ç i m e   d ö n ü ş t ü r ü l ü r . 
 
 # # # #   * * K o d * * 
 ` ` ` p y t h o n 
 #   O r i j i n a l   t e s t   e t i k e t l e r i n i   t e k   s ı c a k   k o d l a m a y a   d ö n ü ş t ü r 
 
 y _ t e s t _ o n e _ h o t   =   t o _ c a t e g o r i c a l ( y _ t e s t ,   n u m _ c l a s s e s = 1 0 ) 

### Bölüm 10

#   * * T e s t   S e t i   P e r f o r m a n s l a r ı n ı n   K a r ş ı l a ş t ı r ı l m a s ı   v e   R a p o r l a n m a s ı * * 
 
 # #   * * A m a ç * * 
 A m a ç ,   m o d e l i n   p e r f o r m a n s ı n ı   ü ç   f a r k l ı   t e s t   v e r i   s e t i n d e   d e ğ e r l e n d i r m e k t i : 
 1 .   * * O r i j i n a l   T e s t   S e t i * * 
 2 .   * * M a n i p ü l e   E d i l m i ş   T e s t   S e t i * * 
 3 .   * * B e y a z   D e n g e l i   T e s t   S e t i * * 
 
 # #   * * S o n u ç   Ö z e t i * * 
 |   T e s t   S e t i   |   D o ğ r u l u k   |   K a y ı p   | 
 | - - - - - - - - - - - - - - - - - - - - - - - - - - - | - - - - - - - - - - - | - - - - - - - - - - | 
 |   * * O r i j i n a l   T e s t   S e t i * *   |   * * % 9 4 , 9 2 * *   |   0 , 4 5 8 9   | 
 |   * * M a n i p ü l e   E d i l m i ş   T e s t   S e t i * *   |   * * % 9 8 , 9 5 * *   |   0 , 3 4 6 6   | 
 |   * * B e y a z   D e n g e l i   T e s t   S e t i * *   |   * * % 9 9 , 6 6 * *   |   0 , 3 3 0 8   | 
 
 # #   * * G ö r ü ş l e r * * 
 1 .   * * O r i j i n a l   T e s t   S e t i * * : 
 -   M o d e l ,   o r i j i n a l   v e r i   s e t i n d e   i y i   p e r f o r m a n s   g ö s t e r e r e k   * * % 9 4 , 9 2 * *   d o ğ r u l u k   e l d e   e d i y o r . 
 -   B u ,   m o d e l i n   e ğ i t i m   d a ğ ı l ı m ı n d a n   v e r i l e r i   d o ğ r u   ş e k i l d e   s ı n ı f l a n d ı r m a   y e t e n e ğ i n i   g ö s t e r i y o r . 
 
 2 .   * * İ ş l e n m i ş   T e s t   S e t i * * : 
 -   P a r l a k l ı k   v e   k o n t r a s t   a y a r l a m a l a r ı y l a   m o d e l ,   * * % 9 8 , 9 5 * *   o r a n ı n d a   i y i l e ş t i r i l m i ş   b i r   d o ğ r u l u k   e l d e   e d i y o r . 
 -   B u ,   m o d e l i n   s a ğ l a m   ö z e l l i k l e r i   ö ğ r e n d i ğ i n i   v e   g ö r s e l   o l a r a k   d e ğ i ş t i r i l m i ş   v e r i l e r e   i y i   g e n e l l e m e   y a p t ı ğ ı n ı   g ö s t e r i y o r . 
 
 3 .   * * B e y a z   D e n g e l i   T e s t   S e t i * * : 
 -   B e y a z   d e n g e s i   d ü z e l t m e s i   i ç i n   G r i   D ü n y a   v a r s a y ı m ı n ı n   u y g u l a n m a s ı ,   d o ğ r u l u ğ u   * * % 9 9 , 6 6 * * ' y a   ç ı k a r ı y o r . 
 -   B u ,   n o r m a l i z a s y o n u n   m o d e l i n   g ö r ü n t ü   ö z e l l i k l e r i n i n   y o r u m l a n a b i l i r l i ğ i n i   a r t ı r m a d a k i   e t k i n l i ğ i n i   g ö s t e r i y o r . 
 
 # #   * * İ y i l e ş t i r m e   Ö n e r i l e r i * * 
 # # #   * * F a r k l ı   Y a p ı l a b i l e c e k   Ş e y l e r * * 
 B u   b o r u   h a t t ı n ı   g e l i ş t i r d i ğ i m d e n   b e r i   ( v e y a   b i z   g e l i ş t i r d i ğ i m i z d e n   b e r i ) ,   a l t e r n a t i f   y a k l a ş ı m l a r ı n   k e ş f e d i l e b i l e c e ğ i   b i r k a ç   a l a n   ş u n l a r d ı r : 
 
 1 .   * * M o d e l   G e l i ş t i r m e l e r i * * : 
 -   R e s N e t   v e y a   E f f i c i e n t N e t   g i b i   ö n c e d e n   e ğ i t i l m i ş   m o d e l l e r   k u l l a n m a k   e ğ i t i m i   h ı z l a n d ı r a b i l i r   v e   s o n u ç l a r ı   d a h a   d a   i y i l e ş t i r e b i l i r d i . 
 -   M o d e l e   S E   b l o k l a r ı   v e y a   C B A M   g i b i   d i k k a t   m e k a n i z m a l a r ı   e k l e m e k ,   ö z e l l i k   ç ı k a r m a y ı   i y i l e ş t i r e b i l i r d i . 
 
 2 .   * * V e r i   H a z ı r l a m a * * : 
 -   R a s t g e l e   g ü r ü l t ü   e n j e k s i y o n u   v e y a   a f i n   d ö n ü ş ü m l e r   g i b i   d a h a   ç e ş i t l i   a r t ı r m a   t e k n i k l e r i n i n   u y g u l a n m a s ı ,   g e r ç e k   d ü n y a   d e ğ i ş k e n l i ğ i n i   d a h a   i y i   s i m ü l e   e d e b i l i r d i . 
 -   D i ğ e r   r e n k   d ü z e l t m e   a l g o r i t m a l a r ı y l a   ( ö r n e ğ i n ,   H i s t o g r a m   E ş i t l e m e )   t e s t   e t m e k   e k   i ç g ö r ü l e r   s a ğ l a y a b i l i r d i . 
 
 3 .   * * H i p e r p a r a m e t r e   O p t i m i z a s y o n u * * : 
 -   O p t u n a   v e y a   H y p e r O p t   g i b i   k ü t ü p h a n e l e r l e   s i s t e m a t i k   h i p e r p a r a m e t r e   a y a r l a m a s ı   y a p m a k   d a h a   i y i   y a p ı l a n d ı r m a l a r   s a ğ l a y a b i l i r d i .   -   M o m e n t u m l u   S G D   v e y a   u y a r l a n a b i l i r   o p t i m i z e   e d i c i l e r   ( ö r n .   A d a m W )   g i b i   o p t i m i z e   e d i c i l e r l e   d e n e m e l e r   y a p m a k   p e r f o r m a n s ı   d a h a   d a   i y i   a y a r l a y a b i l i r d i . 
 
 4 .   * * D e ğ e r l e n d i r m e * * : 
 -   Ç a p r a z   d o ğ r u l a m a ,   s o n u ç l a r ı n   v e r i   k ü m e s i n i n   f a r k l ı   b ö l ü m l e r i n d e   t u t a r l ı   o l d u ğ u n d a n   e m i n   o l m a k   i ç i n   k u l l a n ı l a b i l i r d i . 
 -   M o d e l i   t a m a m e n   g ö r ü l m e m i ş   v e r i   k ü m e l e r i n d e   t e s t   e t m e k ,   g e r ç e k   d ü n y a d a k i   u y g u l a n a b i l i r l i ğ i   h a k k ı n d a   d a h a   i y i   b i r   a n l a y ı ş   s a ğ l a y a b i l i r d i . 
 
 # # #   * * P u a n l a r   D ü ş ü k   O l s a y d ı   ( < % 5 0 ) * * 
 D o ğ r u l u k   ö n e m l i   ö l ç ü d e   d a h a   d ü ş ü k   o l s a y d ı ,   a t ı l a b i l e c e k   a d ı m l a r   ş u n l a r d ı r : 
 -   * * M o d e l   B a s i t l e ş t i r m e * * :   M i m a r i y i   b a s i t l e ş t i r e r e k   v e y a   b ı r a k m a   k a t m a n l a r ı   e k l e y e r e k   a ş ı r ı   u y u m u   a z a l t m a . 
 -   * * A r t t ı r m a * * :   A ş ı r ı   u y u m u   ö n l e m e k   v e   g e n e l l e m e y i   i y i l e ş t i r m e k   i ç i n   d a h a   a g r e s i f   a r t ı r m a l a r   s u n m a . 
 -   * * İ n c e   A y a r * * :   T r a n s f e r   ö ğ r e n i m i   k u l l a n ı l a r a k   d a h a   k ü ç ü k   b i r   v e r i   k ü m e s i n d e   e ğ i t i m   v e r m e k ,   d a h a   g ü ç l ü   b i r   t e m e l   o l u ş t u r m a y a   y a r d ı m c ı   o l a b i l i r d i . 
 
 # #   * * S o n u ç * * 
 M o d e l ,   t ü m   t e s t   s e t l e r i n d e   y ü k s e k   d o ğ r u l u k   e l d e   e d e r e k   o l a ğ a n ü s t ü   b i r   g e n e l l e m e   g ö s t e r i y o r .   A n c a k   m i m a r i ,   v e r i   ö n   i ş l e m e   v e   h i p e r p a r a m e t r e   a y a r l a m a l a r ı n d a k i   i y i l e ş t i r m e l e r ,   p e r f o r m a n s ı   d a h a   d a   i l e r i y e   t a ş ı y a b i l i r d i .   B e y a z   d e n g e s i   d ü z e l t m e s i n i n   e t k i l i   b i r   i y i l e ş t i r m e   o l d u ğ u   k a n ı t l a n d ı   v e   t e s t   d o ğ r u l u ğ u n u   ö n e m l i   ö l ç ü d e   a r t ı r d ı .   B u   d e n e y ,   b e n z e r   g ö r e v l e r i n   g e l e c e k t e k i   y i n e l e m e l e r i   i ç i n   s a ğ l a m   b i r   t e m e l   o l u ş t u r u y o r .

## Kod Özeti

Not defterinde aşağıdaki işlevleri uygulayan çeşitli kod hücreleri bulunmaktadır.

### Kod Hücresi 1

```python

# Gerekli kütüphaneleri içe aktar
import cv2
import numpy as np
import os
import shutil
from pathlib import Path

# Veri seti dizinleri (Dosya yapınıza göre ayarlayın)
data_dir = "/kaggle/input/animals-with-attributes-2/Animals_with_Attributes2/JPEGImages"
output_dir = "/kaggle/working/selected_animals_dataset"
processed_dir = "/kaggle/working/processed_dataset"

# Seçilen hayvan sınıfları
selected_classes = [
    "collie", "dolphin", "elephant", "fox", "moose", 
    "rabbit", "sheep", "squirrel

```

* 1 adet çıktı içerir.

### Kod Hücresi 2

```python

# Gerekli Kütüphanelerin İçe Aktarılması
import os
import numpy as np
from sklearn.model_selection import train_test_split

# İşlenmiş Veri Seti Dizini
processed_dir = "/kaggle/working/processed_dataset"

# Seçilen Hayvan Sınıfları
selected_classes = [
    "collie", "dolphin", "elephant", "fox", "moose", 
    "rabbit", "sheep", "squirrel", "giant+panda", "polar+bear"
]

# Veri ve Etiketlerin Hazırlanması
X = []  # Images
y = []  # Labels
class_mapping = {cls: idx for idx, cls in enumerate(select

```

* 1 adet çıktı içerir.

### Kod Hücresi 3

```python

# Gerekli Kütüphanelerin İçe Aktarılması
from tensorflow.keras.preprocessing.image import ImageDataGenerator

# Eğitim Verilerine Veri Artırımı Uygulanması
augmentation = ImageDataGenerator(
    rotation_range=20,  # Rastgele döndürme
    width_shift_range=0.2,  # Yatayda rastgele kaydırma
    height_shift_range=0.2,  # Dikeyde rastgele kaydırma
    shear_range=0.2,  # Kesme dönüşümleri
    zoom_range=0.2,  # Rastgele yakınlaştırma
    horizontal_flip=True,  # Rastgele yatay çevirme
    fill_mod

```

* 1 adet çıktı içerir.

### Kod Hücresi 4

```python

# Görüntü Manipülasyonu Fonksiyonu
def get_manipulated_images(input_dir, output_dir, brightness_factor=1.5, contrast_factor=1.2):
    if not os.path.exists(output_dir):
        os.makedirs(output_dir)
    
    for class_name in os.listdir(input_dir):
        class_path = os.path.join(input_dir, class_name)
        output_class_path = os.path.join(output_dir, class_name)
        
        if not os.path.exists(output_class_path):
            os.makedirs(output_class_path)
        
        for img_

```

* 1 adet çıktı içerir.

### Kod Hücresi 5

```python

# Yolların tanımlanması
manipulated_dir = "/kaggle/working/manipulated_images"  # İşlenmiş veri kümesi dizini
wb_output_dir = "/kaggle/working/wb_corrected_images"  # Beyaz dengeli veri kümesi dizini

# İşlenmiş veri kümesinin yüklenmesi
X_manipulated_train, y_manipulated_train = get_manipulated_images(manipulated_dir, manipulated_images)
print(f"Manipulated dataset loaded: {X_manipulated_train.shape}, {y_manipulated_train.shape}")

# Beyaz dengeli veri kümesinin yüklenmesi
X_wb_train, y_wb_trai

```

* 1 adet çıktı içerir.

### Kod Hücresi 6

```python

# Gerekli Kütüphanelerin İçe Aktarılması
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Conv2D, MaxPooling2D, Flatten, Dense, Dropout, Input, LeakyReLU, BatchNormalization
from tensorflow.keras.optimizers import Adam
from tensorflow.keras.utils import to_categorical
from tensorflow.keras.regularizers import l2
from sklearn.utils import shuffle

# Orijinal, İşlenmiş ve Beyaz Dengeli Veri Kümelerinin Birleştirilmesi
X_combined_train = np.concatenate([X_train, X_

```

* 7 adet çıktı içerir.

### Kod Hücresi 7

```python

# Yüklenen manipüle edilmiş test seti
manipulated_dir = "/kaggle/working/manipulated_images"  # Gerektiği gibi yolu ayarlayın

# İşlenmiş test görüntülerinin ve etiketlerinin yüklenmesi
X_manipulated_test, y_manipulated_test = load_images_from_directory(manipulated_dir, selected_classes)

print(f"Manipulated Test Set Loaded: {X_manipulated_test.shape}, {y_manipulated_test.shape}")

# İşlenmiş test etiketlerini tek sıcak kodlamaya dönüştür
y_manipulated_test_one_hot = to_categorical(y_manipulated

```

* 1 adet çıktı içerir.

### Kod Hücresi 8

```python

# Beyaz dengesi sağlanmış test setinin yüklenmesi
wb_output_dir = "/kaggle/working/wb_corrected_images"  # Gerektiği gibi yolu ayarlayın

# Beyaz dengesi sağlanmış test görüntülerin ve etiketlerin yüklenmesi
X_wb_test, y_wb_test = load_images_from_directory(wb_output_dir, selected_classes)

print(f"White-Balanced Test Set Loaded: {X_wb_test.shape}, {y_wb_test.shape}")

y_wb_test_one_hot = to_categorical(y_wb_test, num_classes=10)

wb_loss, wb_accuracy = model.evaluate(X_wb_test, y_wb_test_one_ho

```

* 1 adet çıktı içerir.

### Kod Hücresi 9

```python

# Orijinal test etiketlerini tek hot codinge dönüştür
y_test_one_hot = to_categorical(y_test, num_classes=10)

# Modeli orijinal test setinde değerlendirin
original_loss, original_accuracy = model.evaluate(X_test, y_test_one_hot, verbose=2)

# Sonuçların Çıktısı
print(f"Original Test Loss: {original_loss}, Original Test Accuracy: {original_accuracy}")

```

* 1 adet çıktı içerir.
