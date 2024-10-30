                                                    # Kick Komutları

| **Komut**                    | **Kullanım**                       | **İşelevi**                                                                                   |
|------------------------------|------------------------------------|------------------------------------------------------------------------------------------------|
| `/ban <username> <reason>`   | Channel Owners, Moderators         | Bans the `<username>` from your channel.                                                        |
| `/unban <username>`          | Channel Owners, Moderators         | Unbans the `<username>` from your channel.                                                      |
| `/timeout <username> <time>` | Channel Owners, Moderators         | Temporarily prevents `<username>` from chatting for a specified time.                           |
| `/clear`                     | Channel Owners, Moderators         | Clears all current chat messages.                                                               |
| `/slow on <seconds>`         | Channel Owners, Moderators         | Enables slow mode, limiting message frequency by `<seconds>`.                                   |
| `/slow off`                  | Channel Owners, Moderators         | Disables the slow mode.                                                                         |
| `/mod <username>`            | Channel Owners                     | Gives `<username>` a moderator role.                                                            |
| `/unmod <username>`          | Channel Owners                     | Removes the moderator role from `<username>`.                                                   |
| `/title <new title>`         | Channel Owners                     | Sets a new title for the current stream.                                                        |
| `/followonly on`             | Channel Owners                     | Only allows followers to chat.                                                                  |
| `/followonly off`            | Channel Owners                     | Disables follow-only chat.                                                                      |
| `/subonly on`                | Channel Owners                     | Only allows subscribers to chat.                                                                |
| `/subonly off`               | Channel Owners                     | Disables subscriber-only chat.                                                                  |
| `/category <new category>`   | Channel Owners, Moderators         | Changes the stream category.                                                                    |
| `/emoteonly <on_off>`        | Channel Owners, Moderators         | Enables or disables emote-only mode.                                                            |
| `/user <username>`           | Channel Owners, Moderators         | Displays information about `<username>`.

                                                      # Botrix Komutları


| **Komut**         | **Açıklama**                                                                             | **Örnek**                    | **Gereklilik**             | **İzin**          |
|-------------------|------------------------------------------------------------------------------------------|------------------------------|----------------------------|--------------------|
| `!followage`      | Kullanıcının kanalı ne kadar süredir takip ettiğini gösterir.                            | `!followage`                 | N/A                        | Herkes            |
| `!followers`      | Yayıncının kaç takipçisi olduğunu gösterir.                                              | `!followers`                 | N/A                        | Herkes            |
| `!uptime`         | Yayıncının ne kadar süredir canlı olduğunu gösterir.                                     | `!uptime`                    | N/A                        | Herkes            |
| `!top`            | En çok destek veren kullanıcıların listesini gösterir.                                   | `!top`                       | Seviye sistemi             | Herkes            |
| `!level`          | Gönderenin seviyesini gösterir.                                                          | `!level`                     | Seviye sistemi             | Herkes            |
| `!xp`             | Yayını en çok destekleyen kullanıcıların listesini gösterir.                             | `!xp`                        | Seviye sistemi             | Herkes            |
| `!watchtime`      | Kullanıcının yayını ne kadar süredir izlediğini gösterir.                                | `!watchtime`                 | Puan sistemi               | Herkes            |
| `!points`         | Gönderenin sahip olduğu puanları gösterir.                                               | `!points`                    | Puan sistemi               | Birden fazla seçenek |
| `!commands`       | Yayıncının sahip olduğu komutların listesini gönderir.                                   | `!commands`                  | N/A                        | Herkes            |
| `!so`             | Başka bir kullanıcının kanalını tanıtır.                                                 | `!so @ninja`                 | N/A                        | Moderatörler      |
| `!editcounter`    | Sayaç değerini düzenler.                                                                 | `!editcounter wins 10`       | N/A                        | Moderatörler      |
| `!poll`           | Sohbette anket oluşturma komutu (daha fazla bilgi için bir sonraki bölüme bakın).        | `!poll create`               | Anket widget’ı             | Birden fazla seçenek |

### 2.2 - Puanlar

| **Argüman**       | **Alt-Argüman** | **Açıklama**                                      | **Örnek**                      | **İzin**      |
|-------------------|-----------------|---------------------------------------------------|--------------------------------|---------------|
| `[name]`          | Yok             | Bir kullanıcının puanlarını kontrol eder.         | `!points @Oyuncaz`             | Herkes        |
| `add`             | `[name]`        | Kullanıcıya puan ekler.                           | `!points add @Oyuncaz 100`     | Moderatörler  |
| `add`             | `all`           | Tüm kullanıcılara puan ekler.                     | `!points add all 100`          | Moderatörler  |

### 2.3 - Anketler

| **Komut**         | **Açıklama**                                                 | **Örnek**                     | **İzin**      |
|-------------------|--------------------------------------------------------------|-------------------------------|---------------|
| `create`          | Anket widget’ını görünür hale getirir.                       | `!poll create`                | Moderatörler  |
| `title`           | Anketin başlığını belirler.                                  | `!poll title Will i win?`     | Moderatörler  |
| `option`          | Seçeneklerden birine oy verilecek değeri ekler.              | `!poll option 1 You will win` | Moderatörler  |
| `start`           | Belirtilen süre için anketi başlatır.                        | `!poll start 120`             | Moderatörler  |
| `vote`            | Belirli bir seçeneğe oy verir.                               | `!poll vote 3`                | Herkes        |
| `reset`           | Mevcut anketi siler.                                         | `!poll reset`                 | Moderatörler  |

### 2.4 - Özel Komutlar

| **Komut**         | **Açıklama**                                                           | **Örnek**                            | **İzin**       |
|-------------------|------------------------------------------------------------------------|--------------------------------------|----------------|
| `!addcom`         | Yeni komut oluşturur, ilk argüman komut adı, ikincisi yanıtıdır.       | `!addcom !so Follow $(variable)...`  | Moderatörler   |
| `!editcom`        | Var olan komutu düzenler, ilk argüman komut adı, ikincisi yanıtıdır.   | `!editcom !ig Follow me on...`       | Moderatörler   |
| `!delcom`         | Mevcut komutu siler.                                                   | `!delcom myoldcommand`               | Moderatörler   |

### 2.5 - Şarkı İsteği

| **Komut**         | **Açıklama**                                                   | **Örnek**                      | **İzin**        |
|-------------------|----------------------------------------------------------------|--------------------------------|-----------------|
| `!sr`             | Kullanıcıların şarkı talep etmesine izin verir.                | `!sr alan walker faded`        | Herkes          |
| `!currentsong`    | Şu anda çalan şarkının başlığını sağlar.                       | `!currentsong`                 | Herkes          |
| `!skipsong`       | Şu anda çalan şarkıyı atlar ve sıradaki şarkıya geçer.         | `!skipsong`                    | Moderatörler    |

### 2.6 - Tahminler

| **Komut**         | **Açıklama**                                                      | **Örnek**                     | **İzin**      |
|-------------------|-------------------------------------------------------------------|-------------------------------|---------------|
| `!bet`            | Belirli bir seçeneğe belirli miktarda puan ile bahis oynar.       | `!bet yes 1000`               | Herkes        |
| `!bet create`     | Moderatörlerin tahminler oluşturmasını sağlar.                    | `!bet create`                 | Moderatörler  |
| `!bet result`     | Moderatörlerin kazanan seçeneği seçmesini sağlar.                 | `!bet result yes`             | Moderatörler  |