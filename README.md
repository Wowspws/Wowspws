local changeAnim = function(OGAnim, NewAnim, NewAnimSpeed, NewAnimTPos)
local player = game.Players.LocalPlayer
    local character = player.Character or player.CharacterAdded:Wait()
    local humanoid = character:WaitForChild("Humanoid")

    humanoid.AnimationPlayed:Connect(function(d)
if d.Animation.AnimationId == "rbxassetid://"..tostring(OGAnim) then
d:Stop()

        local pchar= game.Players.LocalPlayer.Character
        local AnimationId = tostring(NewAnim)
        local Anim = Instance.new("Animation")
        Anim.AnimationId = "rbxassetid://"..AnimationId
        local k = pchar:FindFirstChildOfClass('Humanoid'):LoadAnimation(Anim)
        k:Play()
if NewAnimSpeed then
k:AdjustSpeed(NewAnimSpeed)
end
if NewAnimTPos then
k.TimePosition = NewAnimTPos
end
       end
end)
end




changeAnim(10466974800, 13560306510)

changeAnim(12510170988, 18179181663)

changeAnim(10468665991, 13073745835)

changeAnim(10471336737, 16431491215)

changeAnim(11365563255, 13071982935)

changeAnim(10469493270, 17889458563)

changeAnim(10469630950, 17889461810)

changeAnim(10469639222, 17889471098)

changeAnim(10469643643, 17889290569)

changeAnim(15955393872, 15943915877)

changeAnim(12447707844, 15957376722)

changeAnim(15955393872, 15943915877)
