return (
<div className="min-h-screen bg-gray-950 text-white">
{/_ Header _/}
<header className="sticky top-0 z-50 bg-gray-900 border-b border-gray-800">
<div className="max-w-7xl mx-auto flex items-center justify-between px-4 py-3">
<div className="text-xl font-bold">MotoCitizen</div>
<nav className="space-x-4 hidden md:block">
<a href="#" className="hover:underline">Форум</a>
<a href="#" className="hover:underline">Как помочь</a>
<a href="#" className="hover:underline">Сообщить о ДТП</a>
<a href="#" className="hover:underline">Волонтёры</a>
<a href="#" className="hover:underline">Контакты</a>
</nav>
<Button className="ml-4 bg-red-600 hover:bg-red-700">Сообщить о ДТП</Button>
</div>
</header>

{/_ Hero _/}
<section className="bg-gray-900 py-20 text-center px-6">
<h1 className="text-4xl md:text-5xl font-bold mb-4">Мы первыми приезжаем, когда каждый час на счету</h1>
<p className="text-gray-300 max-w-2xl mx-auto mb-8">
MotoCitizen — сообщество волонтёров, помогающих при мото-ДТП. Мы рядом, когда нужна помощь.
</p>
<div className="space-x-4">
<Button className="bg-red-600 hover:bg-red-700">Сообщить о ДТП</Button>
<Button variant="outline" className="border-gray-600 text-white">Присоединиться</Button>
</div>
</section>

{/_ Latest incidents _/}
<section className="max-w-5xl mx-auto px-4 py-12">
<h2 className="text-2xl font-semibold mb-6">Последние происшествия</h2>
<div className="grid gap-4 md:grid-cols-2">
{[1, 2, 3, 4].map((id) => (
<Card key={id} className="bg-gray-800 border border-gray-700">
<CardContent className="p-4 space-y-2">
<div className="flex items-center text-sm text-gray-400">
<MapPin className="w-4 h-4 mr-2" /> Москва, МКАД 47 км
</div>
<div className="flex items-center text-sm text-gray-400">
<Clock className="w-4 h-4 mr-2" /> 15 минут назад
</div>
<div className="flex items-center text-sm text-yellow-400">
<AlertCircle className="w-4 h-4 mr-2" /> Нужна помощь
</div>
<Button size="sm" variant="outline" className="border-gray-600 text-white mt-2">
Подробнее
</Button>
</CardContent>
</Card>
))}
</div>
</section>

{/_ Footer _/}
<footer className="bg-gray-900 border-t border-gray-800 py-8 text-center text-gray-500 text-sm">
© 2025 MotoCitizen. Все права защищены.
</footer>
</div>
);
}
