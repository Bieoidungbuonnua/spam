repeat wait()
until game:IsLoaded()
wait()
local TableChat = {"trietlegitstore chấm site caythuegiareuytin nhất vn","trietlegitstore chấm site caythuegiareuytin nhất vn","trietlegitstore chấm site caythuegiareuytin nhất vn"}
spawn(function()
    while wait() do 
        pcall(function()
            game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(TableChat[math.random(0,#TableChat)],"All")
            wait(12)
        end)
    end
end)
