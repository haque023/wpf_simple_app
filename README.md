<Window x:Class="EHealth.Login"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
        xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
        xmlns:local="clr-namespace:EHealth"
        mc:Ignorable="d"
        Title="Login" Height="950" Width="400"
        WindowStartupLocation="Manual"
        Icon="icon.ico"
        Background="AliceBlue"
        >
    <Grid>
        
        <StackPanel VerticalAlignment="Top" >
            <Image Source="login_back.jpg" Height="250" 
                   Stretch="Fill"
                   HorizontalAlignment="Stretch"/>
            <TextBlock Text="EHealth Service" FontSize="16" FontWeight="Bold" 
            HorizontalAlignment="Center" Margin="0,10,0,0"/>
        </StackPanel>

        <StackPanel VerticalAlignment="Center" Margin="20">
            <TextBlock Text="LOG IN" FontSize="14" FontWeight="Bold" Margin="0,0,0,10"/>

            <Label Content="Email" />
            <TextBox x:Name="EmailTextBox" Height="30" Padding="5" BorderBrush="Gray" BorderThickness="1" />

            <Label Content="Password" Margin="0,10,0,0"/>
            <PasswordBox x:Name="PasswordBox" Height="30" Padding="5" BorderBrush="Gray" BorderThickness="1" />
            <StackPanel Orientation="Horizontal" HorizontalAlignment="Left" Margin="0,10,0,0">
                <TextBlock Text="Forgot Password?" Foreground="Green" Cursor="Hand"/>
                <TextBlock x:Name="LoginFailedTextBlock" Text=" Login failed!" Foreground="Red" Visibility="Collapsed" Margin="10,0,0,0"/>
            </StackPanel>

            <Button Content="Log In" Background="Green" Foreground="White" Height="40" 
         FontWeight="Bold" Margin="0,10,0,0" Click="Button_Click"/>
            <TextBlock x:Name="sessionend" Text="Your session has timed out, please log in again." Foreground="OrangeRed" FontWeight="Bold" Visibility="Collapsed" TextAlignment="Center" Margin="0,50,0,0"/>


        </StackPanel>
    </Grid>
</Window>
