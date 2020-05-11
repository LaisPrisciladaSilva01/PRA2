
import androidx.annotation.NonNull;
import androidx.annotation.Nullable;
import androidx.room.Columninfo;
import androidx.room.Entity;
import androidx.room.PrimaryKey; 

@Entity(tableName = "softs")

public class SoftSkill {

private int sId;
private String sCreationDate;
private String sName;
private String sLearningSituation;
private int sLevel;

@PrimaryKey(autoGenerate = true)
@NonNull
@ColumnInfo(name = "softsId")
private int sId;

@Nullable
@ColumnInfo(name = "softsName")
private String sName;

public SoftSkill(@Nullable String creationDate, String name, String learningSituation) {
sCreationDate = creationDate;
sName = name;
sLearningSituation = learningSituation;
}

public int getId( ) {
return sId;
}

public void setId(int id) {
sId = id;
}

public String getCreationDate( ) {
return sCreationDate;
}

public void setCreationDate(String creationDate) {
sCreationDate = creationDate;
}

public String getName( ) {
return sName;
}

public void setName(String name) {
sName = name;
}

public String getLearningSituation( ) {
return sLearningSituation;
}

public void setLearningSituation(String learningSituation) {
sLearningSituation = learningSituation;
}

public int getLevel( ) {
return sLevel;
}

public void setLevel(int level) {
sLevel = level;
}

private int sLevel;
private String sCreationDate;

}
