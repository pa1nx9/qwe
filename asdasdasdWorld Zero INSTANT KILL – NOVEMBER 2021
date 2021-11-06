local player = game.Players.LocalPlayer
workspace.Mobs.ChildAdded:Connect(function(v)
    wait(0.2)
    while wait() and v:IsDescendantOf(workspace) do
        pcall(function()
            v.Collider.CFrame = player.Character.HumanoidRootPart.CFrame * CFrame.new(0, -8, 0)
        end)
    end
end)
for i, v in next, workspace.Mobs:GetChildren() do
    coroutine.wrap(function()
        while wait() and v:IsDescendantOf(workspace) do
            pcall(function()
                v.Collider.CFrame = player.Character.HumanoidRootPart.CFrame * CFrame.new(0, -8, 0)
            end)
        end
    end)()
end
