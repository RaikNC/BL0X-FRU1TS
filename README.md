-- Carregar a biblioteca OrionLib
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

-- Criar a janela principal
local Window = OrionLib:MakeWindow({Name = "RaikHub - Blox Fruits", HidePremium = false, SaveConfig = true, ConfigFolder = "RaikHubConfig", IntroText = "RaikHub"})

-- Combate
local CombatTab = Window:MakeTab({
    Name = "Combate",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

CombatTab:AddButton({
    Name = "Auto Attack",
    Callback = function()
        autoAttack()
    end    
})

CombatTab:AddButton({
    Name = "Auto Defend",
    Callback = function()
        autoDefend()
    end    
})

CombatTab:AddButton({
    Name = "Increase Damage",
    Callback = function()
        increaseDamage()
    end    
})

CombatTab:AddButton({
    Name = "Reduce Damage Taken",
    Callback = function()
        reduceDamageTaken()
    end    
})

CombatTab:AddButton({
    Name = "One Hit Kill",
    Callback = function()
        oneHitKill()
    end    
})

-- Movimento
local MovementTab = Window:MakeTab({
    Name = "Movimento",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

MovementTab:AddButton({
    Name = "Teleport to Island",
    Callback = function()
        teleportToIsland("IslandName")
    end    
})

MovementTab:AddButton({
    Name = "Fast Travel",
    Callback = function()
        fastTravel("Destination")
    end    
})

MovementTab:AddButton({
    Name = "Fly Mode",
    Callback = function()
        flyMode()
    end    
})

MovementTab:AddButton({
    Name = "Increase Speed",
    Callback = function()
        increaseSpeed()
    end    
})

MovementTab:AddButton({
    Name = "Decrease Speed",
    Callback = function()
        decreaseSpeed()
    end    
})

-- Recursos
local ResourcesTab = Window:MakeTab({
    Name = "Recursos",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

ResourcesTab:AddButton({
    Name = "Infinite Fruits",
    Callback = function()
        infiniteFruits()
    end    
})

ResourcesTab:AddButton({
    Name = "Auto Collect Fruits",
    Callback = function()
        autoCollectFruits()
    end    
})

ResourcesTab:AddButton({
    Name = "Increase Fruit Drop Rate",
    Callback = function()
        increaseFruitDropRate()
    end    
})

ResourcesTab:AddButton({
    Name = "Auto Sell Fruits",
    Callback = function()
        autoSellFruits()
    end    
})

ResourcesTab:AddButton({
    Name = "Show Fruit Locations",
    Callback = function()
        showFruitLocations()
    end    
})

-- Habilidades
local SkillsTab = Window:MakeTab({
    Name = "Habilidades",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

SkillsTab:AddButton({
    Name = "Unlock All Skills",
    Callback = function()
        unlockAllSkills()
    end    
})

SkillsTab:AddButton({
    Name = "Increase Skill Damage",
    Callback = function()
        increaseSkillDamage()
    end    
})

SkillsTab:AddButton({
    Name = "Reduce Skill Cooldown",
    Callback = function()
        reduceSkillCooldown()
    end    
})

SkillsTab:AddButton({
    Name = "Auto Use Skills",
    Callback = function()
        autoUseSkills()
    end    
})

SkillsTab:AddButton({
    Name = "Show Skill Info",
    Callback = function()
        showSkillInfo()
    end    
})

-- Proteção
local ProtectionTab = Window:MakeTab({
    Name = "Proteção",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

ProtectionTab:AddButton({
    Name = "God Mode",
    Callback = function()
        godMode()
    end    
})

ProtectionTab:AddButton({
    Name = "Auto Heal",
    Callback = function()
        autoHeal()
    end    
})

ProtectionTab:AddButton({
    Name = "Shield Mode",
    Callback = function()
        shieldMode()
    end    
})

ProtectionTab:AddButton({
    Name = "Reduce Damage Taken From Players",
    Callback = function()
        reduceDamageTakenFromPlayers()
    end    
})

ProtectionTab:AddButton({
    Name = "Anti Kill",
    Callback = function()
        antiKill()
    end    
})

-- Informações
local InfoTab = Window:MakeTab({
    Name = "Informações",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

InfoTab:AddButton({
    Name = "Show Player Info",
    Callback = function()
        showPlayerInfo()
    end    
})

InfoTab:AddButton({
    Name = "Show Island Info",
    Callback = function()
        showIslandInfo()
    end    
})

InfoTab:AddButton({
    Name = "Show Fruit Info",
    Callback = function()
        showFruitInfo()
    end    
})

InfoTab:AddButton({
    Name = "Show Skill Info",
    Callback = function()
        showSkillInfo()
    end    
})

InfoTab:AddButton({
    Name = "Show Game Stats",
    Callback = function()
        showGameStats()
    end    
})

-- Funções de exemplo
function autoAttack()
    print("Auto Attack ativado")
end

function autoDefend()
    print("Auto Defend ativado")
end

function increaseDamage()
    print("Increase Damage ativado")
end

function reduceDamageTaken()
    print("Reduce Damage Taken ativado")
end

function oneHitKill()
    print("One Hit Kill ativado")
end

function teleportToIsland(islandName)
    print("Teleportando para " .. islandName)
end

function fastTravel(destination)
    print("Viajando rapidamente para " .. destination)
end

function flyMode()
    print("Modo de voo ativado")
end

function increaseSpeed()
    print("Aumentando velocidade")
end

function decreaseSpeed()
    print("Diminuindo velocidade")
end

function infiniteFruits()
    print("Frutas infinitas ativadas")
end

function autoCollectFruits()
    print("Coletando frutas automaticamente")
end

function increaseFruitDropRate()
    print("Aumentando taxa de drop de frutas")
end

function autoSellFruits()
    print("Vendendo frutas automaticamente")
end

function showFruitLocations()
    print("Mostrando localização das frutas")
end

function unlockAllSkills()
    print("Desbloqueando todas as habilidades")
end

function increaseSkillDamage()
    print("Aumentando dano das habilidades")
end

function reduceSkillCooldown()
    print("Reduzindo tempo de recarga das habilidades")
end

function autoUseSkills()
    print("Usando habilidades automaticamente")
end

function showSkillInfo()
    print("Mostrando informações sobre habilidades")
end

function godMode()
    print("Modo deus ativado")
end

function autoHeal()
    print("Curando automaticamente")
end

function shieldMode()
    print("Modo escudo ativado")
end

function reduceDamageTakenFromPlayers()
    print("Reduzindo dano recebido de jogadores")
end

function antiKill()
    print("Prevenindo morte instantânea")
end

function showPlayerInfo()
    print("Mostrando informações sobre jogadores")
end

function showIslandInfo()
    print("Mostrando informações sobre ilhas")
end

function showFruitInfo()
    print("Mostrando informações sobre frutas")
end

function showGameStats()
    print("Mostrando estatísticas do jogo")
end

-- Função para mover o menu
local UserInputService = game:GetService("UserInputService")
local dragging
local dragInput
local dragStart
local startPos

local function update(input)
    local delta = input.Position - dragStart
    MainFrame.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
end

MainFrame.InputBegan:Connect(function(input)
    if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
        dragging = true
        dragStart = input.Position
        startPos = MainFrame.Position

        input.Changed:Connect(function()
            if input.UserInputState == Enum.UserInputState.End then
                dragging = false
            end
        end)
    end
end)

MainFrame.InputChanged:Connect(function(input)
    if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
        dragInput = input
    end
end)

UserInputService.InputChanged:Connect(function(input)
    if input == dragInput and dragging then
        update(input)
    end
end)

-- Botão para fechar e reabrir o menu
local ToggleButton = Instance.new("TextButton")
ToggleButton.Name = "ToggleButton"
ToggleButton.Parent = ScreenGui
ToggleButton.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
ToggleButton.Position = UDim2.new(0, 0, 0.5, 0)
ToggleButton.Size = UDim2.new(0, 50, 0, 50)
ToggleButton.Font = Enum.Font.SourceSans
ToggleButton.Text = "🍪"
ToggleButton.TextColor3 = Color3.fromRGB(255,
