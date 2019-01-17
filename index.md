<html>
<head>
<title>パスワード認証</title>
</head>
<body>

<?php
    $pass = "1234";                // パスワード設定
    if($_POST['pass'] !== $pass) {        // パスワードチェック
        // パスワード不一致（パスワード入力フォーム表示）
        echo '<form action="' . $_SERVER['SCRIPT_NAME'] . '" method="POST">';
        echo 'パスワードを入力してください。<br>';
        echo '<input type="password" size="5" name="pass" value="">';
        echo '<input type="submit" value="送信"><br>';
        echo '</form>';
    }
    else {
        // パスワード一致
        echo 'ようこそ！！';
    }
?>

</body>
</html>
