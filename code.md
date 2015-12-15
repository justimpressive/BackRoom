import java.util.Random;

public class BackRoom {
	private int itemCabinet = 0;
	private int itemChest = 0;
	private int itemBox = 0;
	
	private boolean lockCabinet = false;
	private boolean lockChest = false;
	private boolean lockBox = false;
	
	Random rando = new Random();
	
	public int getCabinet() {
		return itemCabinet;
	}
	
	public void setCabinet(int theItemCabinet) {
		theItemCabinet = rand.nextInt(4);
		this.itemCabinet = theItemCabinet;
	}
	
	public int getChest() {
		return itemChest;
	}
	
	public void setCabinet(int theItemChest) {
		theItemChest = rand.nextInt(10);
		this.itemChest = theItemChest;
	}
	
	public int getBox() {
		return itemBox;
	}
	
	public void setBox(int theItemBox) {
		theItemBox = rand.nextInt(5);
		this.itemBox = theItemBox;
	}
	
	public boolean lockedCabinet(boolean theLockCabinet) {
		if this.itemCabinet == 0){
			requiredItem = false;
		}else{
			requiredItem = true;
		}
		this.lockedCabinet = requiredItem;
		return this.requiredItem;
	}
	
	public boolean lockedChest(boolean theLockChest) {
		if this.itemChest == 0){
			requiredItem = false;
		}else{
			requiredItem = true;
		}
		this.lockedChest = requiredItem;
		return this.requiredItem;
	}
	
	public boolean lockedBox(boolean theLockBox) {
		if this.itemBox == 0){
			requiredItem = false;
		}else{
			requiredItem = true;
		}
		this.lockedBox = requiredItem;
		return this.requiredItem;
	}
	
	public String toString(){
		String message = "";
		
		message = message + "Chance of finding item = " + this.itemCabinet + "\n";
		message = message + "Chance of finding item = " + this.itemChest + "\n";
		message = message + "Chance of finding item = " + this.itemBox + "\n";
		return message;
	}
}
