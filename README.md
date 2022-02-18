Shit talk macro for dahood lol, keybind is V 
local words = {
    'ur bad',
    'ur dog🐶',
    'aim left faster then your dad🍼',
    'my grandma is better then you',
    'clowned🤡',
    'sonned🤓',
    'your dog water🐶🌊', 
    'son ur dog quit crying', 
    'my grandmother can aim better',
    'you are actual dog get airshot buddy',
    'bro isnt a clown hes the entire circus🤡🍿🍦🎪🎈',
    'bro isnt a clown nor the circus dude is the entire comical industry🤡🍿🎪🎈',
    'you suck bro', 
    'wyd bro aiming is ez 😅', 
    'dude why are u so bad😂😂',
    'dude quit being free', 
    'ur clowning bro wyd🥱',
    'just aim dude😑',
    'bro 100 pumped the wall😂',
    'bro the wall must hurt rn😞',
    'rodent🐭', 
    'no one likes u🤨', 
    'you were so close! better luck next time!😣', 
    'XD😂', 
    'no skill😮',
    'why do u even try😂',
    'if the body is 70% water how are u 100% salt 🤨', 
    './e dab', 
    'time to take out the trash! 🙄🗑', 
    'im surprised you havent rage quit yet😂', 
    'bro quit crying and get better😴', 
    'haha I won🤓🤓', 
    'trash🗑', 
    'ez', 
    'salty', 
    'did you get worse?🤨',
    'why are u still trying bro😂', 
    'dude just quit already😂', 
    'looolloolloololl', 
    'bro has bipolar aim 🤡🤓', 
    '😴😴😴😴',
}
local player = game.Players.LocalPlayer
local keybind = 'v'

local event = game.ReplicatedStorage.DefaultChatSystemChatEvents.SayMessageRequest

player:GetMouse().KeyDown:connect(function(key)
    if key == keybind then
        event:FireServer(words[math.random(#words)], "All")
    end
end) 
