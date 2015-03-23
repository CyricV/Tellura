/**
 * 
 */
package gmail.cyricv.com;

import net.minecraft.entity.passive.EntityCow;
import net.minecraft.init.Items;
import net.minecraft.item.ItemStack;
import net.minecraftforge.event.entity.living.LivingDropsEvent;
import scala.util.Random;
import cpw.mods.fml.common.eventhandler.SubscribeEvent;

/**
 * @author Paden Atkinson
 *
 */
public class DropHandler {
	public static Random random;
	public static int dropped;
	
	@SubscribeEvent
	public void onEntityDrop(LivingDropsEvent event)
	{
		random = new Random();
		dropped = random.nextInt(2) + 1;
		
		if(event.entityLiving instanceof EntityCow) {
			event.entityLiving.entityDropItem(new ItemStack(Items.apple), dropped);
		}
	}
}
