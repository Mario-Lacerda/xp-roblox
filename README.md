# Desafio Dio -  Crie uma experiência no Roblox


## **Projeto: Criando uma experiência no Roblox**

1 - **Programas necessários:**

- Roblox Studio



**Códigos:**

O código a seguir cria uma experiência simples do Roblox com um cubo que gira:

lua

```lua
local cube = Instance.new("Part")
cube.Name = "Cube"
cube.Size = Vector3.new(1, 1, 1)
cube.Position = Vector3.new(0, 1, 0)
cube.Anchored = true

local rotationSpeed = 10

function cubeRotation()
    cube.CFrame = cube.CFrame * CFrame.Angles(0, rotationSpeed * math.rad(dt), 0)
end

game:GetService("RunService").Heartbeat:Connect(cubeRotation)
```



#### **Como usar o código:**

1. Abra o Roblox Studio.
2. Crie uma nova experiência.
3. Cole o código acima na janela de script.
4. Clique no botão **Executar**.



#### **O que o código faz:**

O código cria um cubo e o posiciona no mundo. O código também define uma função que gira o cubo em torno do eixo y a uma velocidade especificada. A função é conectada ao evento Heartbeat, que é chamado a cada quadro. Isso faz com que o cubo gire continuamente.



#### **Observações:**

- Você pode alterar o tamanho, a posição e a velocidade de rotação do cubo alterando os valores nas variáveis `cube.Size`, `cube.Position` e `rotationSpeed`.
- Você pode adicionar mais objetos e scripts à sua experiência para torná-la mais complexa.
- Você pode publicar sua experiência no Roblox para que outras pessoas possam jogá-la.





## 2 - **Programa:** Blender



**Código:** Python

**Script para importar um modelo 3D personalizado para o Roblox Studio:**

python

```python
import bpy
import roblox

# Caminho para o arquivo do modelo 3D
model_path = "caminho/para/o/modelo.fbx"

# Importa o modelo para o Blender
bpy.ops.import_scene.fbx(filepath=model_path)

# Obtém o objeto do modelo
model_object = bpy.context.selected_objects[0]

# Cria um novo material para o modelo
material = bpy.data.materials.new(name="Material do modelo")

# Define a cor do material
material.diffuse_color = (1, 0, 0)

# Atribui o material ao modelo
model_object.data.materials.append(material)

# Exporta o modelo para um formato de arquivo compatível com o Roblox
export_path = "caminho/para/o/modelo.fbx"
bpy.ops.export_scene.fbx(filepath=export_path)

# Cria uma nova instância do Roblox
roblox = roblox.Roblox()

# Faz login no Roblox
roblox.login("nome_de_usuário", "senha")

# Cria um novo jogo no Roblox
game = roblox.create_game("Nome do jogo")

# Importa o modelo para o jogo
model_id = roblox.import_model(export_path)

# Adiciona o modelo ao jogo
roblox.add_model_to_game(game.id, model_id)

# Publica o jogo
roblox.publish_game(game.id)
```



#### **Observações:**

- Você precisará substituir "caminho/para/o/modelo.fbx" pelo caminho real para o arquivo do modelo 3D.
- Você precisará substituir "Nome do jogo" pelo nome que deseja dar ao seu jogo Roblox.
- Você precisará substituir "nome_de_usuário" e "senha" pelas suas credenciais de login do Roblox.

Este script importará o modelo 3D personalizado para o Roblox Studio, criará um novo material para o modelo, exportará o modelo para um formato de arquivo compatível com o Roblox, criará um novo jogo no Roblox, importará o modelo para o jogo e publicará o jogo.





## **Metodo de construção**



#### **Como criar jogos Roblox:**

1. **Abra o Roblox Studio.**
2. **Clique no botão \**Criar novo\**.**
3. **Selecione um modelo para o seu jogo.**
4. **Clique no botão \**Criar\**.**
5. **Comece a criar seu jogo!**



Você pode usar as ferramentas no Roblox Studio para criar seu mundo, adicionar objetos e personagens e escrever scripts para controlar o comportamento do jogo.



#### **Aqui estão algumas dicas para criar jogos Roblox:**

- **Comece pequeno.** Não tente criar um jogo muito complexo em seu primeiro projeto.
- **Use os recursos disponíveis.** O Roblox Studio possui uma ampla variedade de ferramentas e recursos para ajudá-lo a criar seu jogo.
- **Aprenda com os outros.** Existem muitos recursos online e comunidades onde você pode aprender sobre o desenvolvimento de jogos Roblox.
- **Seja criativo!** O Roblox oferece infinitas possibilidades para criar jogos únicos e divertidos.



#### **Aqui estão alguns jogos Roblox populares que você pode criar:**

- **Jogos de aventura:** Explore mundos diferentes, resolva quebra-cabeças e lute contra inimigos.
- **Jogos de construção:** Crie seus próprios mundos e estruturas.
- **Jogos de corrida:** Corra contra outros jogadores ou contra o relógio.
- **Jogos de tiro:** Atire em inimigos e complete missões.
- **Jogos de RPG:** Crie seu próprio personagem e embarque em uma jornada épica.



#### **Depois de criar seu jogo, você pode publicá-lo no Roblox para que outras pessoas possam jogá-lo.**



#### **Observações:**

- O Roblox Studio é gratuito para usar.
- Você pode encontrar muitos tutoriais e recursos online para ajudá-lo a aprender como criar jogos Roblox.
- Seja paciente e persistente. Criar jogos Roblox pode ser desafiador, mas também é muito recompensador.





### **Programas:**

- Roblox Studio
- Blender
- GIMP
- Audacity



#### **Códigos:**

- Lua (linguagem de script do Roblox)
- Python
- C++
- HTML
- CSS



#### **Apps:**

- Roblox Mobile
- Roblox Player
- Roblox Creator Companion
- Roblox Studio Mobile



#### **Como usar esses programas, códigos e apps para criar uma experiência no Roblox:**



- **Roblox Studio:** Use o Roblox Studio para criar e editar experiências do Roblox.
- **Blender:** Use o Blender para criar modelos e animações 3D para suas experiências do Roblox.
- **GIMP:** Use o GIMP para criar e editar imagens para suas experiências do Roblox.
- **Audacity:** Use o Audacity para criar e editar áudio para suas experiências do Roblox.
- **Lua:** Use a linguagem de script Lua para programar suas experiências do Roblox.
- **Python:** Use Python para criar scripts e plugins para suas experiências do Roblox.
- **C++:** Use C++ para criar plugins de alto desempenho para suas experiências do Roblox.
- **HTML:** Use HTML para criar interfaces de usuário personalizadas para suas experiências do Roblox.
- **CSS:** Use CSS para estilizar as interfaces de usuário personalizadas de suas experiências do Roblox.
- **Roblox Mobile:** Use o Roblox Mobile para jogar experiências do Roblox em seu dispositivo móvel.
- **Roblox Player:** Use o Roblox Player para jogar experiências do Roblox em seu computador.
- **Roblox Creator Companion:** Use o Roblox Creator Companion para criar e gerenciar suas experiências do Roblox em seu dispositivo móvel.
- **Roblox Studio Mobile:** Use o Roblox Studio Mobile para criar e editar experiências do Roblox em seu dispositivo móvel.



#### **Observações:**

- Você não precisa usar todos esses programas, códigos e apps para criar uma experiência no Roblox.
- Você pode usar os programas, códigos e apps que melhor se adequam às suas necessidades e habilidades.
- Há muitos recursos disponíveis online para ajudá-lo a aprender como usar esses programas, códigos e apps.





### **Vide site:**

https://tecnobits.com/pt/como-colocar-roblox-em-tela-cheia-no-pc/

https://clubedovideogame.com.br/melhores-jogos-do-roblox/

https://create.roblox.com/
