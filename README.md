if not _G.ExecutedTackleSpeed then
_G.ExecutedTackleSpeed = true
game.Players.LocalPlayer.Character.HumanoidRootPart.ChildAdded:Connect(function(v)
if v.Name == "TackleVelocity" and v then
v.Velocity = v.Velocity * _G.TackleSpeed
end
end)
end
