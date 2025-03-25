repeat wait()
until game:IsLoaded()
wait()
local TableChat = {"caythuegiareuytin nhất vn","MinhTriet","trietlegitstore chấm site"}
spawn(function()
    while wait() do 
        pcall(function()
            game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(TableChat[math.random(0,#TableChat)],"All")
            wait(12)
        end)
    end
end)
