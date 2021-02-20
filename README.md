local function esp(part)
    local billgui = Instance.new('BillboardGui', part)
    local textlab = Instance.new('TextLabel', billgui)

    billgui.Name = "ESP"
    billgui.Adornee = part
    billgui.AlwaysOnTop = true
    billgui.ExtentsOffset = Vector3.new(0, 1, 0)
    billgui.Size = UDim2.new(0, 5, 0, 5)
    
    textlab.Name = 'RUSHED (kill)'
    textlab.BackgroundColor3 = Color3.new(255, 50, 255)
    textlab.BackgroundTransparency = 1
    textlab.BorderSizePixel = 0
    textlab.Position = UDim2.new(0, 0, 0, -40)
    textlab.Size = UDim2.new(1, 0, 10, 0)
    textlab.Visible = true
    textlab.ZIndex = 10
    textlab.Font = 'ArialBold'
    textlab.FontSize = 'Size14'
    textlab.Text = "LEAT (KILL)\nV"
    textlab.TextColor3 = Color3.fromRGB(205,98,152)
    textlab.TextStrokeColor3 = Color3.fromRGB(0,0,0)
    textlab.TextStrokeTransparency = 0.6
end

game.Players.PlayerAdded:Connect(function(plr)
    if plr:IsInGroup(8016146) or plr:IsInGroup(8016146) or plr:IsInGroup(8016146) or plr:IsInGroup(8016146) or plr:IsInGroup(8016146) then
        plr.CharacterAdded:Connect(function(char)
            repeat wait() until char:FindFirstChild("Humanoid")
            repeat wait() until char:FindFirstChild("Head")
            esp(char:FindFirstChild("Head"))
        end)
    end
end)

for i,plr in pairs(game.Players:GetPlayers()) do
    if plr:IsInGroup(8016146) or plr:IsInGroup(8016146) or plr:IsInGroup(8016146) or plr:IsInGroup(8016146) or plr:IsInGroup(8016146) then
        plr.CharacterAdded:Connect(function(char)
            repeat wait() until char:FindFirstChild("Humanoid")
            repeat wait() until char:FindFirstChild("Head")
            esp(char:FindFirstChild("Head"))
        end)
    end
end
