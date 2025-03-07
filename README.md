-- Exploit para spawnar Twisted no Dandy's World

-- Função para spawnar o Twisted
function spawnTwisted()
    -- Verifica se o jogo permite o spawn de entidades
    if canSpawnEntity("Twisted") then
        -- Cria o Twisted na posição especificada (x, y, z)
        local x, y, z = getPlayerPosition()  -- Posição do jogador
        createEntity("Twisted", x + 5, y, z) -- Coloca o Twisted perto do jogador
        print("Twisted spawned successfully!")
    else
        print("Não é possível spawnar Twisted neste momento.")
    end
end

-- Executa a função
spawnTwisted()
